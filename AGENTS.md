# AGENTS.md

Instructions for agents maintaining this list.

## What this repo is

A curated list of ESPHome **external components**: code you pull in with
[`external_components:`](https://esphome.io/components/external_components#git) that does something mainline ESPHome can't.

- `README.md` is the list.
- `ARCHIVE.md` holds entries that no longer qualify. They stay because they're useful references for people learning to write components.

## What "awesome" means here

The test: **would an ESPHome user be glad to find this, and would it work if they added it today?**

The second half is mostly mechanical. The first half is judgment. Use the signals below as evidence, not as a scoring formula.

### Hard requirements (any failure means it doesn't belong on the list)

1. **It's an external component with its own code.** The repo (or the linked subdirectory) contains `components/<name>/__init__.py` plus C++ sources.
   - A YAML config that only uses mainline components (`modbus`, `uart`, lambdas) is not a component, however nice it is.
   - Old-style "custom components" (a `.h` pulled in with `includes:` and a lambda) don't count. ESPHome removed support for them in 2025.2.
2. **Mainline doesn't already do it.** When ESPHome ships an equivalent, the entry graduates and moves to the archive.
   - A repo that overrides a mainline component (shipping its own `ethernet` or `stepper`, say) is fine. What counts is whether the *headline* feature exists in mainline.
   - **Partial graduation:** if mainline has only landed part of it (for example, "part 1: bus core"), keep the entry and note it in the report. Archive it once mainline covers what most users would use it for.
3. **It can work today.** It isn't archived on GitHub, and it isn't known to be broken on current ESPHome (no open "broken since 20xx.y" issues left unanswered).
4. **It isn't mainly a funnel to a commercial cloud.** Components that exist to send data to a vendor's paid platform go against the spirit of the list: local control, getting things out of the cloud. Promotion by itself isn't disqualifying. A vendor publishing a local-control component for their own hardware is welcome.

### Signals of awesome (weigh them, don't add them up)

- **Novelty:** it reaches hardware, a protocol or an ecosystem ESPHome otherwise can't, especially through reverse engineering. Published protocol notes are a strong plus.
- **Escaping the cloud:** it replaces a vendor app, dongle or cloud service with local control.
- **Quality:** a README with a working example YAML, tested-on-hardware claims, CI that compiles against a recent ESPHome.
- **Maintenance:** issues and PRs get responses. Commits help, but a finished component for an unchanging protocol may not need any.
- **Usage:** stars, forks, forum mentions. Treat this as supporting evidence only. A brand-new 3-star repo can be awesome, and a 1,000-star repo can still fail the hard requirements.

### Red flags (look closer, don't auto-reject)

- A fork with few commits ahead of an upstream that's still active: link the upstream instead.
- A repo with one commit (a code dump): fine if the code is good, but you can't judge maintenance yet.
- The description just repeats the name ("ESPHome NUT Server Component"), or is marketing copy.
- Overlap with an existing entry or a mainline component that the entry doesn't explain.

## Badges

- 💤 **Stale:** no commits touching the component's code in over 18 months. It stays on the list, because stale isn't the same as broken.
- If a 💤 component is also archived on GitHub or known to be broken, it moves to the archive.

## Entry format

```markdown
* [Display Name](https://github.com/owner/repo): One sentence on what it lets you do.
```

- Link to **where the component code lives**. If a project repo only holds YAML and points at a separate components repo, link the components repo.
- **Multi-component repos:** list each component that qualifies as its own entry, in the right section, linking to `tree/<branch>/components/<name>`. Don't link several entries to the same repo root.
- The display name is the component's name or the device it supports. Every entry needs a distinct name.
- The description says what it lets you *do* ("Control your…", "Read … over BLE"), in one sentence, without restating the name.
- Put 💤 before the link: `* 💤 [Name](…)`.

## Archiving

Move the line to the matching section of `ARCHIVE.md` and append `_(archived YYYY-MM)_`:

- **Graduated to mainline:** add "Use mainline [`name`](docs link) instead."
- **Old-style custom components**
- **YAML configs, not components**
- **Abandoned:** archived on GitHub, deleted, or broken with no response.

Remove a README section once it has no entries left.

Entries that never belonged (vendor funnels, thin forks) are removed outright, not archived.

## How to check things

```bash
# Repo health
gh api repos/OWNER/REPO --jq '[.archived,.pushed_at,.stargazers_count,.fork,.parent.full_name]'
# Last commit touching one component
gh api "repos/OWNER/REPO/commits?per_page=1&path=components/NAME" --jq '.[0].commit.committer.date'
# Components in a repo
gh api "repos/OWNER/REPO/git/trees/BRANCH?recursive=1" --jq '.tree[].path|select(test("components/[^/]+/__init__\\.py$"))'
# Mainline component list (dev branch; also check release notes for anything just added)
gh api "repos/esphome/esphome/contents/esphome/components?ref=dev" --jq '.[].name'
```

`pushed_at` only tells you about the repo as a whole. For multi-component repos, check commits on the component's own path.

## What agents may do

- **Maintenance sweeps:** edit `README.md` and `ARCHIVE.md` directly and commit to `master`, one targeted commit per kind of change (typos, relinks, archiving, badges). Commit messages say what moved and why.
- **Judgment calls** (red flags, partial graduation, anything in "Signals"): list them in the sweep report for a human to decide. Don't act on them.
- **Pull requests (future):** review submissions against this file, leave feedback that points to the specific rule, and merge when every hard requirement passes and nothing is a red flag. Until that's switched on, draft reviews only. Don't post them.
- Don't open PRs or issues on component repos.

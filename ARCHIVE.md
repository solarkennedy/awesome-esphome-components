# Archive

Components that used to be on the [main list](README.md) but no longer qualify.
They're kept here because they're still great reading if you're learning to write your own ESPHome components.

Each entry notes why it left the list and when.

## Graduated to mainline

These are now built into ESPHome. Use the mainline version instead.

* [syslog](https://github.com/TheStaticTurtle/esphome_syslog): Have your ESPHome device log out via the standard syslog protocol. Use mainline [`syslog`](https://esphome.io/components/syslog/) instead. _(archived 2026-11)_
* [OpenTherm](https://github.com/olegtarasov/esphome-opentherm): Control your OpenTherm-based thermostat from ESPHome. Use mainline [`opentherm`](https://esphome.io/components/opentherm/) instead. _(archived 2026-11)_
* [Hi-Link mmWave Radar](https://github.com/patrick3399/Hi-Link_mmWave_Radar_ESPHome): Support for Hi-Link LD class millimeter wave radar modules. Use mainline [`ld2410`](https://esphome.io/components/sensor/ld2410/), [`ld2420`](https://esphome.io/components/sensor/ld2420/) or [`ld2450`](https://esphome.io/components/sensor/ld2450/) instead. _(archived 2026-11)_
* [mitsubishiheatpump](https://github.com/geoffdavis/esphome-mitsubishiheatpump): Interface with your Mitsubishi Heatpump for automated climate control. Use mainline `mitsubishi_cn105` instead. _(archived 2026-11)_

## Old-style custom components

ESPHome removed support for "custom components" (a `.h` file pulled in with `includes:` and a lambda) in 2025.2, so these no longer build.

* [mipurifier](https://github.com/jaromeyer/mipurifier-esphome): Component for Xiaomi Air Purification devices. _(archived 2026-11)_
* [jura coffee](https://github.com/ryanalden/esphome-jura-component): Control your Jura Impressa class coffee machines. _(archived 2026-11)_

## YAML configs, not components

These are device configs built from mainline components (`modbus`, `uart`, lambdas) rather than external components with their own code.

* [deye](https://github.com/klatremis/esphome-for-deye): Monitor and control your Deye inverters. _(archived 2026-11)_
* [powmr-hybrid-inverter](https://github.com/odya/esphome-powmr-hybrid-inverter): Monitor and control various PowMr Inverter modules. _(archived 2026-11)_
* [smg-ii](https://github.com/syssi/esphome-smg-ii): Monitor and control a iSolar/EASUN SMG II inverter. _(archived 2026-11)_

## Abandoned

* [Roomba Bridge](https://github.com/solarkennedy/roomba-bridge-esphome): Control your Roomba using ESPHome without the internet or the app. Repo archived by its author. _(archived 2026-11)_

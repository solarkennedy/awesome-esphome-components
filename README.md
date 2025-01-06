# Awesome ESPHome Components

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A list of ESPHome components that are too cool to exist in mainline.

To use any of these components in _your_ ESPHome device, check out the documentation for adding [external components](https://esphome.io/components/external_components#git).

**Contributing:**

Know if a cool ESPHome component that is missing?
Please make a PR!

# Components

## Network Hardware

* [TI wMBus](https://github.com/SzczepanLeon/esphome-components): For interfacing with TI's [Wireless M-Bus](https://www.ti.com/tool/WMBUS).

## Network Protocols

* [Telnet Server](https://github.com/RoboMagus/esphome-telnet-server): Adds a telnet bridge so that you can send and receive characters on the serial bus.
* [syslog](https://github.com/TheStaticTurtle/esphome_syslog): Have your ESPHome device log out via the standard syslog protocol.
* [Homekit](https://github.com/rednblkx/HAP-ESPHome): Make your ESPHome devices show up in your Apple Home app.

## Bluetooth/BLE

* [OpenHaystack](https://github.com/barrenechea/esphome-config-files/tree/main/components/openhaystack): Puts your ESPHome device onto the Apple Find My network ([blog](https://www.barrenechea.cl/en/projects/openhaystack-esphome/)).
* [BLE Keyboard](https://github.com/dmamontov/esphome-blekeyboard): Make your ESPHome device a virtual BLE keyboard.

## Distance / Presence Sensors

* [Hi-Link mmWave Radar](https://github.com/patrick3399/Hi-Link_mmWave_Radar_ESPHome): Support for Hi-Link LD class millimeter wave radar modules.

## Electricity Sensors

* [emporia-vue](https://github.com/emporia-vue-local/esphome): Support for the Emporia Vue 2 energy monitor.
* [JK-BMC](https://github.com/syssi/esphome-jk-bms): Interfaces with the Jikong Battery Management System over UART or BLE.
* [p1reader](https://github.com/psvanstrom/esphome-p1reader): For interfacing with the Swidish P1 energy meters.
* [pipsolar](https://github.com/syssi/esphome-pipsolar): Monitor and control a Pipsolar inverter via RS232.
* [deye](https://github.com/klatremis/esphome-for-deye): Monitor and control your Deye inverters.
* [powmr-hybrid-inverter](https://github.com/odya/esphome-powmr-hybrid-inverter): Monitor and control various PowMr Inverter modules.
* [smg-ii](https://github.com/syssi/esphome-smg-ii): Monitor and control a iSolar/EASUN SMG II inverter.
* [VictronMPPT](https://github.com/KinDR007/VictronMPPT-ESPHOME): Monitor and control a Victron Charge Controller

## Environment

* [mitsubishiheatpump](https://github.com/geoffdavis/esphome-mitsubishiheatpump): Interface with your Mitsubishi Heatpump for automated climate control.
* [panasonic-ac](https://github.com/DomiStyle/esphome-panasonic-ac): Interface with your Panasonic Air Conditioner without their "cloud".
* [ecodan](https://github.com/gekkekoe/esphome-ecodan-hp): Interface with your Ecodan heatpump.
* [aux_ac](https://github.com/GrKoR/esphome_aux_ac_component): Direct wifi control of your AUX based air conditioners.
* [OpenTherm](https://github.com/arthurrump/esphome-opentherm): Control your OpenTherm-based thermostat from ESPHome.
* [econet](https://github.com/esphome-econet/esphome-econet):  Controlling a Rheem water heater or HVAC system.
* [Samsung HVAC](https://github.com/omerfaruk-aran/esphome_samsung_hvac_bus): Integrate with Samsung HVACs that use the NASA and NonNASA protocols.
* [Nibe](https://github.com/elupus/esphome-nibe): Control your Nibe Heat Pump over Modbus.
* [lg-controller](https://github.com/JanM321/esphome-lg-controller): Control your LG Air Conditioner instead of the LG ThinQ integration.
* [mipurifier](https://github.com/jaromeyer/mipurifier-esphome): Component for Xiaomi Air Purification devices.

## Light

* [xiaomi_bslamp2](https://github.com/mmakaay/esphome-xiaomi_bslamp2): Integrate with your Xiaomi Mijia Bedside Lamp v2.
* [desky](https://github.com/ssieb/esphome_components/tree/master/components/desky): Component for controlling your Desky standing desk.
* [Yeelight-ceiling-light](https://github.com/syssi/esphome-yeelight-ceiling-light): Control many different models of Yeelight or Xiaomi lights.
* [dmx512](https://github.com/andyboeh/esphome-dmx512): Control DMX devices via a RS485 UART.

## Garage / Security

* [DSCKeyBus](https://github.com/Dilbert66/esphome-dsckeybus): For interfacing with a DSC POWERSERIES alarm system.
* [Konnected](https://github.com/konnected-io/konnected-esphome): Bridge your Konnected alarm system or garage door openers.
* [ratgdo](https://github.com/ratgdo/esphome-ratgdo): Enable sending commands to your garage door opener via your ESPHome device.
* [vistaECP](https://github.com/Dilbert66/esphome-vistaECP): Control your Honeywell/Ademco Vista ECP security system.
* [Nuki Lock](https://github.com/uriyacovy/ESPHome_nuki_lock): Seamless integration of Nuki Smartlocks into ESPHome / Home Assistant.

## Vacuums

* [Roomba Bridge](https://github.com/solarkennedy/roomba-bridge-esphome): Control your Roomba using ESPHome without the internet or the app.

## Misc Appliances

* [Philips-Smart-Coffee](https://github.com/TillFleisch/ESPHome-Philips-Smart-Coffee): Control your Philips Series 2200/3200 Coffee Machines.
* [jura coffee](https://github.com/ryanalden/esphome-jura-component): Control your Jura Impressa class coffee machines.
* [Tesla BLE](https://github.com/yoziru/esphome-tesla-ble): Interface with your Tesla over BLE.
* [igrill](https://github.com/bendikwa/esphome-igrill): Read sensors from iGrill and Pulse BBQs.

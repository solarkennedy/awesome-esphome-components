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
* [uart-link](https://github.com/nebulous/esphome-uart-link): Present TCP connections as virtual UARTs for any UART consumer, bridge them to hardware UARTs, and share one serial bus between multiple TCP clients.
* [syslog](https://github.com/TheStaticTurtle/esphome_syslog): Have your ESPHome device log out via the standard syslog protocol.
* [Homekit](https://github.com/rednblkx/HAP-ESPHome): Make your ESPHome devices show up in your Apple Home app.
* [LoRaWAN](https://github.com/moellere/lorawan-for-esphome): Join a LoRaWAN network over OTAA and uplink any ESPHome sensor's values, using RadioLib for the radio + MAC. For SX127x/SX126x radios.
* [HydroNode](https://github.com/TexhFexLabs/hydronode-esphome): Send any ESPHome sensor to the HydroNode platform with HMAC-signed HTTPS uploads, and drive switches and scripts with typed remote commands.
* [ntp-server](https://github.com/tiehfood/esphome-gps-pps-ntp-server): ESPHome GPS NTP server
* [NUT Server](https://github.com/bullshit/esphome-components): ESPHome NUT Server Component
* [SIP](https://github.com/n-IA-hane/esphome-voip-stack): ESPHome VoIP Stack
  
## Bluetooth/BLE

* [OpenHaystack](https://github.com/barrenechea/esphome-config-files/tree/main/components/openhaystack): Puts your ESPHome device onto the Apple Find My network ([blog](https://www.barrenechea.cl/en/projects/openhaystack-esphome/)).
* [BLE Keyboard](https://github.com/dmamontov/esphome-blekeyboard): Make your ESPHome device a virtual BLE keyboard.
* [Qingping CGG3](https://github.com/OperKH/esphome-qingping-cgg3): Read temperature, humidity and battery level from the Qingping Temp & RH Monitor (CGG3) E-Ink thermometer over BLE, no bindkey needed.
* [BLE ADV](https://github.com/Skrucz/esphome-components): ESPHome for various Chinese lamps that are controlled via BLE advertising
  
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
* [VictronMPPT](https://github.com/KinDR007/VictronMPPT-ESPHOME): Monitor and control Victron Devices such as a Solar Charge Controller.
* [UPS HID Component](https://github.com/bullshit/esphome-components): UPS HID Component
* [dlms-cosem](https://github.com/latonita/esphome-dlms-cosem): ESPHome integration for DLMS/COSEM (SPODES) electricity meters (Energomera CE207/CE307/CE308, Milur 107S, MIR, Nartis, RiM, Pulsar, Aidon, Kamstrup, Landis+Gyr, any HAN, ZPA AM375, ZPA ZE312, Sagemcom XT211 and many others) via RS‑485 or optical port (*).
* [mercury200.2](https://github.com/shammysha/esphome-mercury-200-2): ESPHome integration mercury 200.2
* [apc-ups](https://github.com/samoswall/esphome-apc-ups): ESPHome component to monitor and control a APC UPS via RS232 with MQTT
  
## Environment

* [mitsubishiheatpump](https://github.com/geoffdavis/esphome-mitsubishiheatpump): Interface with your Mitsubishi Heatpump for automated climate control.
* [panasonic-ac](https://github.com/DomiStyle/esphome-panasonic-ac): Interface with your Panasonic Air Conditioner without their "cloud".
* [panasonic-erv](https://github.com/ShadowZZP/esphome-panasonic-erv): Control your Panasonic ERV / fresh-air heat-recovery ventilator (新风) over its private CN12 bus, no cloud or OEM module needed.
* [ecodan](https://github.com/gekkekoe/esphome-ecodan-hp): Interface with your Ecodan heatpump.
* [aux_ac](https://github.com/GrKoR/esphome_aux_ac_component): Direct wifi control of your AUX based air conditioners.
* [OpenTherm](https://github.com/olegtarasov/esphome-opentherm): Control your OpenTherm-based thermostat from ESPHome.
* [OpenTherm-otgw](https://github.com/mvdnes/esphome-otgw): ESPHome OpenTherm Gateway The OTGW project can be found here: https://otgw.tclcode.com/
* [OpenTherm-otgw](https://github.com/gduteil/OpenThermGateway): ESPHome OpenTherm Gateway I'm using this hardware DIYLESS OpenTherm Gateway
* [OpenTherm-otgw](https://github.com/KPWhiver/opentherm-gateway-esphome): This is an external esphome component to control a Nodoshop Opentherm Gateway.
* [econet](https://github.com/esphome-econet/esphome-econet):  Controlling a Rheem water heater or HVAC system.
* [Samsung HVAC](https://github.com/omerfaruk-aran/esphome_samsung_hvac_bus): Integrate with Samsung HVACs that use the NASA and NonNASA protocols.
* [Nibe](https://github.com/elupus/esphome-nibe): Control your Nibe Heat Pump over Modbus.
* [lg-controller](https://github.com/JanM321/esphome-lg-controller): Control your LG Air Conditioner instead of the LG ThinQ integration.
* [mipurifier](https://github.com/jaromeyer/mipurifier-esphome): Component for Xiaomi Air Purification devices.
* [HDMI-CEC](https://github.com/Palakis/esphome-native-hdmi-cec): ESPHome devices speak the (machine) language of your living room with this native HDMI-CEC (Consumer Electronics Control) component
* [MIoT](https://github.com/dhewg/esphome-miot): ESPHome components are designed for MIoT devices
* [intercom](https://github.com/n-IA-hane/esphome-intercom): ESP32 intercoms and a provider or PBX trunk.
  
## Light

* [xiaomi_bslamp2](https://github.com/mmakaay/esphome-xiaomi_bslamp2): Integrate with your Xiaomi Mijia Bedside Lamp v2.
* [desky](https://github.com/ssieb/esphome_components/tree/master/components/desky): Component for controlling your Desky standing desk.
* [Yeelight-ceiling-light](https://github.com/syssi/esphome-yeelight-ceiling-light): Control many different models of Yeelight or Xiaomi lights.
* [dmx512](https://github.com/andyboeh/esphome-dmx512): Control DMX devices via a RS485 UART.
* [Matrix Lamp Music Leds / Sound Reactive](https://github.com/andrewjswan/esphome-components): Matrix Lamp Music Leds, Sound Reactive, Giver lamp
* [Adaptive lighting](https://github.com/mdvorak/esphome-adaptive-lighting): Adaptive lighting component for ESPHome. It sets the light color temperature based on the current position of the sun.
* [ujin](https://github.com/ananyevgv/esphome-ujin): Ujin Light device
* [AC Dimmer](https://github.com/InspectorTrinket/advanced_ac_dimmer): An ESPHome external component for AC phase-angle dimming of mains-connected loads. Designed for real-world installations where timing precision, load compatibility, and flicker-free operation matter.
    
## Garage / Security

* [DSCKeyBus](https://github.com/Dilbert66/esphome-dsckeybus): For interfacing with a DSC POWERSERIES alarm system.
* [Konnected](https://github.com/konnected-io/konnected-esphome): Bridge your Konnected alarm system or garage door openers.
* [ratgdo](https://github.com/ratgdo/esphome-ratgdo): Enable sending commands to your garage door opener via your ESPHome device.
* [vistaECP](https://github.com/Dilbert66/esphome-vistaECP): Control your Honeywell/Ademco Vista ECP security system.
* [Nuki Lock](https://github.com/uriyacovy/ESPHome_nuki_lock): Seamless integration of Nuki Smartlocks into ESPHome / Home Assistant.
* [TTLock](https://github.com/bazuchan/esphome-ttlock): This is a set of projects related to using TTLock locks locally with ESPHome
* [homegate](https://github.com/ananyevgv/esphome-homegate): ESPHome gate homegate

## Vacuums

* [Roomba Bridge](https://github.com/solarkennedy/roomba-bridge-esphome): Control your Roomba using ESPHome without the internet or the app.
* [BEAM](https://github.com/ananyevgv/esphome-beam): ESPHome BEAM vacuum cleaner
  
## Actuators

* [TMC2208](https://github.com/slimcdk/esphome-custom-components/blob/master/esphome/components/tmc2208/README.md) & [TMC2209](https://github.com/slimcdk/esphome-custom-components/blob/master/esphome/components/tmc2209/README.md): Component for Trinamic stepper motor drivers

## Vehicles

* [fiido-bms](https://github.com/dzikus/esphome-fiido-bms): Read a Fiido ebike's BMS over BLE and control power, light, gear and speed limit, without the Fiido app.
* [xbot](https://github.com/dzikus/esphome-xbot): Read telemetry and settings from electric scooters built on the OEM XBOT / LebiTEC controller over BLE, and write the settings back.

## Health / Personal Care

* [omron](https://github.com/dzikus/esphome-omron): Pull blood pressure readings out of an Omron BLE cuff's memory, with no Omron cloud account and no phone app.
* [oclean](https://github.com/dzikus/esphome-oclean): Battery, dock state and buffered brushing sessions from an Oclean BLE toothbrush, plus brushing mode, language and brush-head reminder control.

## Misc Appliances

* [pumpsaver](https://github.com/lizbit-official/esphome-pumpsaver): Read live volts/amps/watts, trip settings, and the 20-fault history from a SymCom/Littelfuse PumpSaver well-pump protection relay, passively, over its IR status broadcast.
* [Philips-Smart-Coffee](https://github.com/TillFleisch/ESPHome-Philips-Smart-Coffee): Control your Philips Series 2200/3200 Coffee Machines.
* [jura coffee](https://github.com/ryanalden/esphome-jura-component): Control your Jura Impressa class coffee machines.
* [jura-uart-esphome](https://github.com/harryzz/jura-uart-esphome): Replace the Jura Smart Connect dongle with an ESP32 on the service port: counters, alerts, brew progress, brewing and panel lock over MQTT with HA discovery, using Jura's native dongle protocol and a built-in profile database for 75 machines.
* [Tesla BLE](https://github.com/yoziru/esphome-tesla-ble): Interface with your Tesla over BLE.
* [igrill](https://github.com/bendikwa/esphome-igrill): Read sensors from iGrill and Pulse BBQs.

## Sensor
* [MQ](https://github.com/ananyevgv/esphome-components): ESPHome component MQ gaz sensor
* [PM1006k](https://github.com/ananyevgv/esphome-components): ESPHome component PM1006k
* [Anemometer](https://github.com/ananyevgv/esphome-components): ESPHome component anemometer sensor
* [Radsens](https://github.com/krbaker/esphome-radsens): ESPHome component for radiation sensor
* [jhm1200](https://github.com/DJTerentjev/esphome_jhm1200): ESPHome component for pressure sensor
 
## Sniffer
* [i2c](https://github.com/hencou/esphome_components): Sniffer i2c

## Timer
* [dynamic-on-time](https://github.com/hostcc/esphome-component-dynamic-on-time): Basically, it functions similar to time.on_time trigger, but allows changing the schedule dynamically.

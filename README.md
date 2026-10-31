# X50 Diagnostics вЂ” downloads

Android diagnostics for Belgee X50 / Geely SX11. No root required.

Download APKs and ESP firmware from [Releases](https://github.com/AlteroAscension/x50-diagnostics-releases/releases).
This repository contains public release notes and curated distributable files;
application and firmware source development is in a separate private repository.

Supported adapters: ESP32 / WeAct CAN485 over USB or Bluetooth; ELM327 over Bluetooth
(reading and experimental writes requiring vehicle validation).
Each release lists precisely what was built, tested and still needs hardware
validation. Current preview: **Android 0.4.4 / ESP32 firmware 0.8.4**.
Autonomous CAN-to-microSD recording, sleep/wake boundaries and CAN-date names.
0.8.4 removes40856B of idle static RAM through on-demand output/Launch buffers
and starts Classic SPP without unused BLE. Recording monitor and internal SPP
queues are bounded; diagnostic message/query capacities are retained.
Builds, full host models and both Android emulator interfaces passed. Physical
SD/Bluetooth/overnight operation and correction on the reported board still
require field validation. See [0.4.4 notes and installation](RELEASE_NOTES_0.4.4.md).

The application includes a USB firmware installer. Use only an image matching
your board; disconnect CAN and remove microSD before flashing. Bundled target: ESP32 8MB,
CAN TX27/RX26. C3 and arbitrary ESP32 boards require their own firmware profile.

Related public projects: [Navigation](https://github.com/AlteroAscension/x50-navigation-releases),
[Gateway](https://github.com/AlteroAscension/x50-gateway-releases),
[Media Bridge](https://github.com/AlteroAscension/x50-media-bridge-releases),
[Home Assistant](https://github.com/AlteroAscension/belgee-x50-ha-integration),
[Control Center](https://github.com/AlteroAscension/belgee-x50-control-center).

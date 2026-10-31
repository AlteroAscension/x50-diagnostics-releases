# X50 Diagnostics вЂ” downloads

Android diagnostics for Belgee X50 / Geely SX11. No root required.

Download APKs and ESP firmware from [Releases](https://github.com/AlteroAscension/x50-diagnostics-releases/releases).
This repository contains public release notes and curated distributable files;
application and firmware source development is in a separate private repository.

Supported adapters: ESP32 / WeAct CAN485 over USB or Bluetooth; ELM327 over Bluetooth
(reading and experimental writes requiring vehicle validation).
Each release lists precisely what was built, tested and still needs hardware
validation. Current preview: **Android 0.4.3 / ESP32 firmware 0.8.3**.
Autonomous CAN-to-microSD recording, sleep/wake file boundaries, CAN-date filenames
and RAM budgeting for the `257 / mount` failure are included. Queue capacity
adapts to leave room for the contiguous FAT/VFS block, SD drivers and Bluetooth.
Builds, host models and emulator checks passed; physical SD/overnight operation
and correction of the reported mount failure still require field validation.
See [0.4.3 notes and installation](RELEASE_NOTES_0.4.3.md).

The application includes a USB firmware installer. Use only an image matching
your board; disconnect CAN and remove microSD before flashing. Bundled target: ESP32 8MB,
CAN TX27/RX26. C3 and arbitrary ESP32 boards require their own firmware profile.

Related public projects: [Navigation](https://github.com/AlteroAscension/x50-navigation-releases),
[Gateway](https://github.com/AlteroAscension/x50-gateway-releases),
[Media Bridge](https://github.com/AlteroAscension/x50-media-bridge-releases),
[Home Assistant](https://github.com/AlteroAscension/belgee-x50-ha-integration),
[Control Center](https://github.com/AlteroAscension/belgee-x50-control-center).

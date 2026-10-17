# X50 Diagnostics — downloads

Android diagnostics for Belgee X50 / Geely SX11. No root required.

Download APKs and ESP firmware from [Releases](https://github.com/AlteroAscension/x50-diagnostics-releases/releases).
This repository contains public release notes and curated distributable files;
application and firmware source development is in a separate private repository.

First target: ESP32 / WeAct CAN485 over USB or Bluetooth; ELM327 reader support.
ESP32-C3 firmware and BLE support are planned, not yet released as working.
Each release lists precisely what was built, tested and still needs hardware
validation. First release is a preview; phone/vehicle testing is pending.

The application includes a USB firmware installer. Use only an image matching
your board; disconnect CAN before flashing. Initial bundled target: ESP32 8MB,
CAN TX27/RX26. C3 and arbitrary ESP32 boards require their own firmware profile.

Related public projects: [Navigation](https://github.com/AlteroAscension/x50-navigation-releases),
[Gateway](https://github.com/AlteroAscension/x50-gateway-releases),
[Media Bridge](https://github.com/AlteroAscension/x50-media-bridge-releases),
[Home Assistant](https://github.com/AlteroAscension/belgee-x50-ha-integration),
[Control Center](https://github.com/AlteroAscension/belgee-x50-control-center).

# X50 Diagnostics - downloads

Android diagnostics for Belgee X50 / Geely SX11. No root required.

Download APKs and ESP firmware from [Releases](https://github.com/AlteroAscension/x50-diagnostics-releases/releases).
This repository contains public release notes and curated distributable files;
application and firmware source development is in a separate private repository.

Supported adapters: ESP32 / WeAct CAN485 over USB or Classic Bluetooth SPP;
WeAct CANFD ESP32-C5 over native USB CDC or BLE UART; ELM327 over Bluetooth
(reading and experimental writes requiring vehicle validation).
Each release lists precisely what was built, tested and still needs hardware
validation. Current preview: **Android 0.4.12 / CAN485 0.8.10 / C5 0.1.0**.
Late CAN-clock filename updates now run after recording stops and its queue drains.
DTC lists support up to2048 bytes through ESP and ELM. Optional monitor losses
are separate from critical replies; idle read-session recovery preserves counters
and never clears an unknown mutation outcome. The opt-in HU policy remains
up to3 attempts with3-second pauses; CAN opens in normal mode with ACK.
Builds, full host models, exact bundled-image ROM model and both Android emulator
interfaces passed. The new build still requires physical SD/vehicle validation.
CAN485 HU autostart now continues when SD is absent or fails; update the board
to0.8.10 to apply this fix. Existing CAN/engine/ACC/door checks and the3-attempt
limit remain. The release includes separate C5 adapter, host diagnostics/keys,
USB/BLE settings and guarded USB installer. C5 has no SD or autonomous HU wake.
Physical C5 USB/BLE/CAN/LED/flashing and the new CAN485 build need field checks.
See [0.4.12 notes and installation](RELEASE_NOTES_0.4.12.md).

The application includes a USB firmware installer. Use only an image matching
your board; disconnect CAN and, for CAN485, remove microSD before flashing.
Separate bundled targets: CAN485 ESP32 8MB (TX27/RX26) and WeAct CANFD ESP32-C5
(TX23/RX24, native USB CDC). C3 and arbitrary boards require their own profile.

Related public projects: [Navigation](https://github.com/AlteroAscension/x50-navigation-releases),
[Gateway](https://github.com/AlteroAscension/x50-gateway-releases),
[Media Bridge](https://github.com/AlteroAscension/x50-media-bridge-releases),
[Home Assistant](https://github.com/AlteroAscension/belgee-x50-ha-integration),
[Control Center](https://github.com/AlteroAscension/belgee-x50-control-center).

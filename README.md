# Dell Latitude E5570 & Dell Precision 3510 OpenCore
## Overview

This EFI has been tested on Mac OS 13 `Ventura` Mac OS 14 `Sonoma` and Mac OS 15 `Sequoia`.


## Specs

| Part             | Description                                                                                                    |
| ---------------- | -------------------------------------------------------------------------------------------------------------- |
| CPU              | Intel® Core™ i7-6820HQ Processor (will most likely work on other variants too)                                 |
| iGPU             | Intel® HD 530 & AMD Radeon™ R7 M370                                                                            |
| Memory           | 32Gb (2 x 16Gb 2400MHz) (should work fine with 8gb+)                                                           |
| Storage          | SSD 512gb NVMe (should work fine with SATA SSD's too)                                                          |
| Display          | 15.6 inch 1920x1080 IPS Matte Panel                                                                            |
| Wifi & Bluetooth | Intel® Dual-Band Wireless-AC 8265                                                                              |
| LAN              | Intel® Gigabit Ethernet, 10/100/1000                                                                           |
| Audio            | Realtek ALC3235                                                                                                |
| External ports   | 1 x USB Type C Thunderbolt 3, 3 x USB 3.0, 1 x Ethernet, 1 x SD Card Reader, 1 x HDMI 1.4, 1 x 3.5 headphone/microphone combo, 1 x VGA |

### Working and Not Working

|                                                   | Status | Note                              |
| ------------------------------------------------- | ------ | ----------------------------------|
| Keyboard (with volume keys and brightness control keys) | ✅     |                                   |
| Touchpad with all gestures and buttons            | ✅     |                                   |
| Ethernet                                          | ✅     |                                   |
| Wifi                                              | ✅     |Intel only with [Heliport](https://github.com/OpenIntelWireless/HeliPort) on Sequoia |
| Bluetooth                                         | ✅     |                                   |
| SD Card Reader                                    | ✅     |                                   |
| Camera & Mic                                      | ✅     |                                   |
| Speaker & 3.5mm audio port                        | ✅     |                                   |
| Intel iGPU & VGA & HDMI                           | ✅     |Spoofed to HD 630 for native support  |
| AMD Radeon™ R7 M370                               | ❌     |Disabled due to not being supported past Monterey        |
| USB                                               | ✅     |                                   |
| Sleep                                             | ✅     |                                   |
| Handoff                                           | ✅     |                                   |
| Thunderbolt                                       | ✅     |                                   |
| Airdrop                                           | ❌     |                                   |


## Usage

Download my EFI, Change your Serial with [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) and install.

If installing Sequoia using Intel wifi you'll need to download [Heliport](https://github.com/OpenIntelWireless/HeliPort)

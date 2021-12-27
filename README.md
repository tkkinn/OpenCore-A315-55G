# OpenCore ACER A315-55G

![banner](banner.png)

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)



__My Specs__

| Specs | Details |
|------------|-------------------------------|
| Model | Acer Aspire 3 A315-55G-51C1 |
| OS | macOS Monterey && Windows 11  |
| CPU | Intel(R) Core(TM) i5 i5-10210U |
| RAM | 8 GB DDR4 2666MHz |
| iGPU | Intel UHD Graphics 620 |
| dGPU | NVIDIA GeForce MX230 |
| Wireless | Dell Wireless 1820A |
| Audio | ALC255 |

__Tested and working__

- [x] Intel UHD Graphics 620
- [x] USB
- [x] Webcam
- [x] LAN
- [x] Screen brightness
- [x] Battery status
- [x] Sleep/Wake
- [x] WiFi
- [x] Bluetooth
- [x] HDMI + HDMI Audio
- [x] Airdrop + Handoff
- [x] Audio + Headphone + Internal Mic
- [x] Keyboard (Some function keys not work)
- [x] iServices
- [x] TouchPad with gestures 

__Not working__

- [ ] NVIDIA GeForce MX230


## Guide

__BIOS Settings__

- Set Supervisor Password
- Disable Secure Boot
- Disable CFG Lock

__OpenCore config__

- Follow these instructions to configure your OpenCore: https://dortania.github.io/OpenCore-Install-Guide/  
- ACPI Hotpatch: https://github.com/daliansky/OC-little  
- Audio layout ID 71

__Install MacOS__

- Create bootable USB: https://dortania.github.io/OpenCore-Install-Guide/installer-guide/  
- If you have problems installing Catalina or later. Install Mojave then you can update to newer version.

__USB Mapping__

- USB Mapping: https://github.com/corpnewt/USBMap

__Fix iServices__

- Fix iServices: https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html


__Fix Dual Boot__

- Fix timezone: https://www.tonymacx86.com/threads/fix-incorrect-time-in-windows-osx-dual-boot.133719/  

__UEFI Secure Boot__

- Setting: https://tkkinn.gitbook.io/opencore-uefi-secureboot-guide/


## Disclaimer

According to Apple Inc., use this EFI to run macOS or OSX on a non-Apple-branded computer as known as "Hackintosh" are illegal, per the [Digital Millenium Copyright Act](https://www.copyright.gov/dmca/). In addition, creating a "Hackintosh" computer violates [Software License Agreement](https://www.apple.com/legal/sla/docs/macOSMonterey.pdf) for any operating systen in the OSX family.

If you use this EFI for commercial or public use, you may be arrested by local law enforcement agencies or sued by Apple Inc. **This EFI is for educational use only**.

If you choose to use this EFI, it means that you agree to take the risk of using this EFI. This EFI is unstable, it may break your laptop and need to send it in for repair. I'm not responsile for any loss caused by the use of this EFI. **USE IN YOUR OWN RISK**

## Credits

Thanks to Acidanthera, RehabMan, dortania, alexandred, daliansky

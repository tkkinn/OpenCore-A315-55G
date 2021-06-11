# OpenCore EFI for Acer A315-55G

[香港繁體 README](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/README_zh-hk.md)

## Important
**This EFI only support OpenCore** instead of CLOVER  
You should edit `config.plist` when you are using Coffee Lake (8th Generation)  
This EFI theoretically supports the Acer A315-55G, but was only tested on the Acer A315-55G-51C1 (Comet Lake).   
Maybe it can be supported on other models.

## Disclaimer
Your warranty may void. I am not responsible for any loss, including but not limited to Kernel Panic, device fail to boot or can not function normally, storage damage or data loss, and so on.

## What doesn't work
Qualcomm Atheros QCA9377 Wireless Network Adapter  
(It is recommended to replace with Dell Wireless 1820A)  
dGPU: NVIDIA GeForce MX230 2GB GDDR5  
I2C HID Touchpad (DSDT lost too much imformation)

## Current Version
OpenCore 0.6.9  
MacOS Big Sur 11.3.1  
  
Big Sur 11.4 and Monterey 12.0 Developer Beta 1 are not tested, but that does not mean they are not supported.  

## Coffee Lake
`SSDT-PMC.aml` is not required for 8th gen laptops.  
You should delete this file from /OC/ACPI and also delete `SSDT-PMC.aml` in `config.plist`.  
If you still do not know what ACPI you need, you should read [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#acpi).

## DW1820A
Make sure you are using DW1820A, otherwise you should delete the following kext from /OC/kext and also delete the following kext in `config.plist`  

BrcmBluetoothInjector.kext  
BrcmFirmwareData.kext  
BrcmPatchRAM3.kext  
AirportBrcmFixup.kext  
AirPortBrcm4360_Injector.kext  
AirPortBrcmNIC_Injector.kext  

## Testing Platform
Acer A315-55G-51C1  
- CPU : 
  * Intel Core i5-10210U Processor 6M Cache, up to 4.20 GHz  
- Wifi :
  * Qualcomm Atheros QCA9377 Wireless Network Adapter 
  * Dell Wireless 1820A
- Graphics: 
  * iGPU: Intel UHD Graphics 620
  * dGPU: NVIDIA GeForce MX230 2GB GDDR5
- Storage:
  * SSD: Kingston 120GB NVMe SSD + Western Digital 2TB
- Keyboard:
  * PS/2 keyboard
  * I2C HID Touchpad  
- Dual Boot:
  * Windows 10
  * MacOS Big Sur 11.3.1


## Thanks
[Acidanthera](https://github.com/acidanthera) - OpenCore and other kext  
[Apple](https://www.apple.com/macos/big-sur/) - macOS  
[alexandred](https://github.com/alexandred) - VoodooI2C  
[daliansky](https://github.com/daliansky) - OC litte  

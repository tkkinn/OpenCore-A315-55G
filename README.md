# OpenCore EFI for Acer A315-55G

[香港繁體](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/README_zh-hk.md)

## Please Read First
This model has four types of CPUs 
-  Intel Core i5-8265U
-  Intel Core i5-10210U
-  Intel Core i3-8145U
-  Intel Core i3-10110U

This EFI has not been tested on 8th gen yet, feel free to create issues in github. 

NVIDIA GPU is not supported, it has been disabled with boot-args `-wegnoegpu` 

After successful installation, you should edit the SMBIOS  
**DO NOT LOGIN YOUR APPLE ID BEFORE YOU EDIT SMBIOS**  

[BIOS Setting](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#intel-bios-settings)  
[Disclaimer](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/Docs/Disclaimer.md)
[Testing Platform](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/Docs/Testing_Platform.md)


## What doesn't work
Qualcomm Atheros QCA9377 Wireless Network Adapter  
NVIDIA GeForce MX230 2GB GDDR5  
  
DW1820A is recommended to replace QCA9377

## Current Version
OpenCore 0.7.0  
MacOS Big Sur 11.3.1  
  
Big Sur 11.4 and Monterey 12.0 Developer Beta 1 are not tested.

## Update 
2021/06/22 Update  
- Update to OpenCore 0.7.0
- Rebuild README and the file system

## Thanks
[Acidanthera](https://github.com/acidanthera) - OpenCore and other kext  
[alexandred](https://github.com/alexandred) - VoodooI2C  
[daliansky](https://github.com/daliansky) - OC litte  

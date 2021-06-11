# Acer A315-55G EFI 引導檔案
[ENGLISH README](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/README.md)

## 重要須知
**此 EFI 僅支持 OpenCore** 而不是 CLOVER  
使用 Coffee Lake（第 8 代）時應該編輯 `config.plist`   
該 EFI 理論上支持 Acer A315-55G，但僅在 Acer A315-55G-51C1（Comet Lake）上進行了測試。  
也許它可以在其他型號上支持。

## 免責聲明
您的保修可能會失效。我將不對任何損失負責，包括但不限於內核崩潰、設備無法啟動或無法正常運行、存儲損壞或數據丟失等。 

## 當前版本
OpenCore 0.6.9  
MacOS Big Sur 11.3.1

Big Sur 11.4 和 Monterey 12.0 Developer Beta 1 未經過測試，但這並不意味著它們不受支持   

## 什麼沒有工作 
Qualcomm Atheros QCA9377 無線網絡適配器  
（建議更換為 Dell Wireless 1820A）  
dGPU: NVIDIA GeForce MX230 2GB GDDR5  
I2C HID 觸摸板 (DSDT 丟失了太多信息)

## Coffee Lake
第 8 代筆記本電腦不需要 `SSDT-PMC.aml`  
您應該從 /OC/ACPI 中刪除此文件，並刪除 `config.plist` 中的 `SSDT-PMC.aml`。

## DW1820A
請確保您使用的是 DW1820A，否則您應該從 /OC/kext 中刪除以下 kext，並在 `config.plist` 中刪除以下 kext 

BrcmBluetoothInjector.kext  
BrcmFirmwareData.kext  
BrcmPatchRAM3.kext  
AirportBrcmFixup.kext  
AirPortBrcm4360_Injector.kext  
AirPortBrcmNIC_Injector.kext  

## 測試平台
Acer A315-55G-51C1  
- 中央處理器 : 
  * Intel Core i5-10210U Processor 6M Cache, up to 4.20 GHz  
- 無線網絡 :
  * Qualcomm Atheros QCA9377 無線網絡適配器   
  * Dell Wireless 1820A
- 顯卡 : 
  * iGPU: Intel UHD Graphics 620
  * dGPU: NVIDIA GeForce MX230 2GB GDDR5
- 存儲:
  * SSD: Kingston 120GB NVMe SSD + Western Digital 2TB
- 觸摸板:
  * PS/2 鍵盤 
  * I2C HID 觸摸板 
- 雙啟動:
  * Windows 10
  * MacOS Big Sur 11.3.1

## 鳴謝
[Acidanthera](https://github.com/acidanthera) - OpenCore and other kext  
[Apple](https://www.apple.com/macos/big-sur/) - macOS  
[alexandred](https://github.com/alexandred) - VoodooI2C  
[daliansky](https://github.com/daliansky) - OC litte  

# Acer A315-55G EFI 引導檔案
[英文](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/README.md)

## 請先閱讀
這個型號有四種類型的CPU
- i5-8265U
- i5-10210U
- i3-8145U
- i3-10110U

EFI 引導檔案尚未在第八代上測試，請隨時在此github上創建問題。

不支持NVIDIA GPU，它已經被boot-args `-wegnoegpu` 禁止。

安裝成功後，你應該編輯SMBIOS
**在編輯SMBIOS之前不要登錄你的蘋果ID**。

[BIOS設置](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#intel-bios-settings)  
[免責聲明](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/Docs/Disclaimer_zh-hk.md)  
[測試平台](https://github.com/tkkinn/OpenCore-A315-55G/blob/main/Docs/Testing_Platform_zh-hk.md)  

## 什麼沒有工作
Qualcom Atheros QCA9377 無線網絡連接  
NVIDIA GeForce MX230 2GB GDDR5  
    
QCA9377 建議更換為 DW1820A  

## 當前版本
OpenCore 0.7.0
MacOS Big Sur 11.3.1

Big Sur 11.4 和 Monterey 12.0 Developer Beta 1 未經測試 但這並不意味著它們不受支持

## 更新
2021/06/22 更新
- 更新至OpenCore 0.7.0

## 鳴謝
[Acidanthera](https://github.com/acidanthera) - OpenCore 和其他 kext  
[alexandred](https://github.com/alexandred) - VoodooI2C  
[daliansky](https://github.com/daliansky) - OC litte   

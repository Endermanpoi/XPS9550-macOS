# XPS9550-Mojave

参考[大佬的教程和资料](https://github.com/darkhandz/XPS-9550-Mojave)自行修改的

### 配置:

* CPU:i7-6700HQ
* 内存:4GB DDR4 2133 *2
* 显卡:HD530 + GTX960m（然并卵）
* 屏幕:4K（1080P可以直接用，不需要改）
* 网卡:DW1830
* 硬盘:960PRO 512GB

### 分区:

Win10和macOS双系统:

* macOS:100GB APFS
* Win10:100GB NTFS
* 资料盘:300+GB exFAT

（便于双系统读写，以4096簇大小格式化，虽然分区表会很大，但存小文件就不会占用太多空间）

### 版本:

* macOS:10.14.6(18G95)
* CLOVER:5070
* AppleALC.kext:1.3.9
* VirtualSMC.kext:1.0.5
* Lilu.kext:1.3.7
* WhateverGreen.kext:1.3.0

### 备注:

10.14的小版本更新都可以无损进行。

变频不管了，用Intel Power Gadget看似乎是正常的，CPU-S不准确（对，一定是这样的）。

Clover从4983开始把默认EFI驱动目录从EFI/CLOVER/drivers64UEFI移动到了EFI/CLOVER/drivers/UEFI。
（我今天才发现的，放在原目录也可以）
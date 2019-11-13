# XPS9550-Mojave

参考[大佬的教程和资料](https://github.com/darkhandz/XPS-9550-Mojave)自行修改的

### 配置:

* CPU:i7-6700HQ
* 内存:4GB DDR4 2133 *2
* 显卡:HD530 + GTX960m（然并卵）
* 屏幕:4K
* 网卡:DW1830
* 硬盘:960PRO 512GB

### 分区:

Win10和macOS双系统:

* macOS:100GB APFS
* Win10:100GB NTFS
* 资料盘:300+GB exFAT

（便于双系统读写，以4096簇大小格式化，虽然分区表会很大，但存小文件就不会占用太多空间）

### 版本:

* macOS:10.14.6(18G1012)
* CLOVER:5098
* AppleALC.kext:1.4.3
* VirtualSMC.kext:1.0.9
* Lilu.kext:1.3.9
* WhateverGreen.kext:1.3.4

### 备注:

10.14的小版本更新都可以无损进行。

1080P版本，在config.plist中启动背景->UI比例改为1，纯文本的话是这里`<key>UIScale</key><integer>2</integer>`

i5版本，引用[大佬的教程](https://github.com/wmchris/DellXPS15-9550-OSX/blob/10.14/Tutorial_10.14.md)

>If your PC has a Core i5 processor, you'll have to modify your config.plist in EFI/CLOVER/: search for the Key ig-platform-id: 0x191b0000 and replace it with 0x19160000. Also search for AAPL,ig-platform-id: AAAbGQ== and change it to AAAWGQ== 

但是在我的config.plist并没有找到前一个修改的地方，需要的童鞋自己研究一下试试看吧
# 铭瑄挑战者 H610ITX 2.5G 黑苹果
Items | Details
--- | ---
CPU | i9 13900 注意，大小核心需要开启所有线程的话，需要禁用SMCProcessor.kext,开启ProvideCurrentCpuInfo
主板 |  MAXSUN H610ITX ([BIOS](https://www.maxsun.com.cn/2022/0512/5728.html):E1.6G)
显卡 | Radeon™ RX 6600 8GB GDDR6
Wifi |  BCM943602CS
内存 | 光威 天策 32GB 3200*2, 主板BIOS限制，目前只能2933，3200需要手动设置更细的参数，懒得折腾了。 
硬盘 | 1TB NVME(MacOS) +1TB SATA(Windows) 
OpenCore | 0.9.5 


注意：Sonoma 14下老的博通无线网卡(BCM943602CS之类)驱动被移除了，现在已经手动加回来了，需要OpenCore-Legacy-Patcher的支持。
EFI里面增加了驱动，不过安装完成后需要OpenCore-Legacy-Patcher执行 Post-Install Root Patch
https://github.com/dortania/OpenCore-Legacy-Patcher
参考：https://www.bilibili.com/read/cv25391191/
使用我的EFI都配置好了，只需要最后一步OpenCore-Legacy-Patcher执行 Post-Install Root Patch

![](AboutMac.png)


 BIOS设置 | 是否启用 
--- | ---
 Hyper-Threading | Enable
 VT-d Enable Above 4G decoding | Enable
 Resizable Bar | Enable
 EHCI/XHCI Hand-off | Enable
 Wake on USB | Enable
 Wake on Bluetooth | Enable
 CFG Lock | Disable
 Security Device Support | Disable
 Serial/COM Port | Disable
 CSM Support | Disable
 Fast Boot | Disable
 Secure Boot | Disable
 Trusted platform Module | Disable
 Wake on LAN | Disable

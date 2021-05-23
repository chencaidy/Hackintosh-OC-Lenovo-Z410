# UEFIPatch for Lenovo Z410

## 特性

* 解锁高级菜单选项
* 解锁 MSR 0xE2 寄存器（CFG Lock）
* 增加无线网卡白名单 Apple BCM94360CS2
* 增加无线网卡白名单 Dell DW1820A（CN_08PKF4）
* 增加无线网卡白名单 Intel AX200
* 修复TSC同步问题导致的macOS异常卡顿

## 操作手册（补丁适用BIOS版本：8DCN40WW）

* 下载[UEFIPatch](https://github.com/LongSoft/UEFITool/releases/download/0.28.0/UEFIPatch_0.28.0_win32.zip)，将UEFIPatch.exe放入此目录。
* 使用编程器提取BIOS固件（4M的BIN文件）。
* 将提取的固件放入此目录，重命名为`bios.bin`。
* 打开CMD运行命令：`UEFIPatch.exe bios.bin`。
* 将生成的`bios.bin.patch`编程器刷入BIOS芯片。

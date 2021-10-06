# Hackintosh-OC-Lenovo-Z410

## 平台配置

* 平台：Lenovo Z410
* CPU：Intel Core i7-4870HQ (Crystal Well)
* iGPU：Intel Iris Pro Graphics 5200
* dGPU：NVIDIA GT740M（已屏蔽）
* 网卡：Dell DW1820A
* 触摸板：Synaptics TM2132
* 显示屏：LTN140HL02
* 内存：16GB

## 特性

* 仿冒机型：MacBookPro11,4（SN已去除，需自行补充）
* 系统版本：Big Sur 11.6
* 显示正常，显卡FB：0D260007，VRAM：1536MB，端口限制：2（去除不存在的0204和0306端口防止开机卡顿）
* 内置扬声器正常，耳机输出正常，声卡ID：51
* WiFi正常，地区#a
* 蓝牙正常，支持接力
* 触摸板正常，多指操作正常
* 键盘正常，支持音量亮度调节
* USB端口正常，去除无效端口，端口属性正确修正
* EC（SMC）正常，支持电量报告
* CPU电源管理正常，支持功率报告
* 电池睡眠正常，适配器供电睡眠正常
* 电源按钮正常，短按1S休眠，长按>3S弹出关机对话框
* 合盖休眠正常

## BIOS配置（版本：8DCN40WW）

* 高级菜单破解：BIOS定制
* 关闭CFG锁：BIOS定制
* TSC同步补丁：BIOS定制
* 恢复出厂设置：`Exit` > `Other OS` > `Load Default Settings`
* 开启VT-x：`Configuration` > `Intel Virtual Technology` > `Enabled`
* 预分配显存128M：`Advanced` > `Video Configuration` > `Internal Graphic Device` > `IGD - DVMT Pre-Allocated` > `128 MB`
* 关闭VT-d：`Advanced` > `Chipset Configuration` > `VT-d` > `Disabled`

## 更新日志

### 2021-10-6

* 更新OpenCore 0.7.4
* 更新AppleALC 1.6.5
* 更新VoodooPS2 2.2.6
* 更新WhateverGreen 1.5.4

### 2021-9-8

* 更新OpenCore 0.7.3
* 更新AirportBrcmFixup 2.1.3
* 更新AppleALC 1.6.4
* 更新BrcmPatchRAM 2.6.0
* 更新BrightnessKey 1.0.2
* 更新Lilu 1.5.6
* 更新VirtualSMC 1.2.7
* 更新VoodooPS2 2.2.5
* 更新WhateverGreen 1.5.3

### 2021-5-24
* 增加BIOS补丁教程

### 2021-5-23

* 更新OpenCore 0.6.9
* 更新AppleALC 1.6.0
* 更新RealtekRTL8111 2.4.2
* 更新Lilu 1.5.3
* 更新VoodooPS2 2.2.3
* 更新VirtualSMC 1.2.3
* 启用开机音效
* 启用图形化UI界面
* 更换网卡为DW1820A

### 2021-3-12

* 修复合盖休眠功能
* 更改显卡FB到0D260007，解决部分页面花屏，需设置128MB预分配显存

### 2021-3-8

* 修复电源按钮功能
* 注入LPC

### 2021-3-7

* 支持按键亮度调节
* 修复睡眠唤醒后自动重启
* 修复睡眠自动唤醒

### 2021-3-6

* 更新OpenCore 0.6.7

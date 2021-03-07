# Hackintosh-OC-Lenovo-Z410

## 平台配置
* 平台：Lenovo Z410
* CPU：Intel Core i7-4870HQ (Crystal Well)
* iGPU：Intel Iris Pro Graphics 5200
* dGPU：NVIDIA GT740M（已屏蔽）
* 网卡：Apple BCM94360CS2
* 触摸板：Synaptics TM2132
* 显示屏：LTN140HL02
* 内存：16GB

## 特性
* 仿冒机型：MacBookPro11,4（SN已去除，需自行补充）
* 系统版本：Big Sur 11.2.2
* 显示正常，显卡FB：0A260005，VRAM：1536MB，端口限制：2（去除不存在的0204端口防止开机卡顿）
* 内置扬声器正常，耳机输出正常，声卡ID：51
* WiFi正常，免驱
* 蓝牙正常，支持接力
* 触摸板正常，多指操作正常
* EC（SMC）正常，支持电量报告
* CPU电源管理正常，支持功率报告

## 已知问题
* 电源按钮无效
* 盒盖休眠无效
* USB端口未修正

## BIOS配置（版本：8DCN40WW）

## 更新日志
### 2021-3-7
* 修复睡眠唤醒后自动重启
* 修复睡眠自动唤醒
### 2021-3-6
* 更新OpenCore 0.6.7

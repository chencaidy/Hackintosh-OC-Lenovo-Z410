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
* 键盘正常，支持音量亮度调节
* USB端口正常，去除无效端口，端口属性正确修正
* EC（SMC）正常，支持电量报告
* CPU电源管理正常，支持功率报告
* 电池睡眠正常，适配器供电睡眠正常

## 已知问题
* 电源按钮无效
* 盒盖休眠无效

## BIOS配置（版本：8DCN40WW）
* 高级菜单破解：BIOS定制
* 关闭CFG锁：BIOS定制
* TSC同步补丁：BIOS定制
* 恢复出厂设置：`Exit` > `Other OS` > `Load Default Settings`
* 开启VT-x：`Configuration` > `Intel Virtual Technology` > `Enabled`
* 预分配显存64M：`Advanced` > `Video Configuration` > `Internal Graphic Device` > `IGD - DVMT Pre-Allocated` > `64 MB`
* 关闭VT-d：`Advanced` > `Chipset Configuration` > `VT-d` > `Disabled`

## 更新日志
### 2021-3-7
* 支持按键亮度调节
* 修复睡眠唤醒后自动重启
* 修复睡眠自动唤醒
### 2021-3-6
* 更新OpenCore 0.6.7

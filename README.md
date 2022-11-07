# UINIO-DAP-Link

一款基于 [**DAP Link**](https://daplink.io/) 的开源 ARM 硬件调试工具电路设计。

![](./Images/PCB-3D-1.png)

![](./Images/PCB-3D-2.png)

- 使用 **USB Type-C** 接口以及贴片晶振；
- 采用 `STM32F103C8T6` 微控制器方案；
- 低压差线性稳压器 **LDO** 调整为 `ME6211C33M5G` 方案；
- 兼容 [ARMmbed DAPLink](https://github.com/ARMmbed/DAPLink/releases/tag/v0257) 提供的 `REL v0257` 最新版固件；
- 提供 **SWD/JTAG** 转换板，以及清晰的符号标识；
- 预留 `1mm` 和 `2mm` 直径固定螺丝孔，方便与外壳进行固定；

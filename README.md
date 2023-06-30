# UINIO-DAP-Link

一款基于开源 [**ARM DAP Link**](https://daplink.io/) 固件的硬件下载调试器电路设计，采用了 `QFT48` 封装的 **STM32F103C8T6** 或者 **STM32F103RBT6** 微控制器，也兼容其它 `Pin to Pin` 的 **Cortex-M3** 微控制器（需要自行修改固件）。

![](./Images/PCB-3D-1.png)

![](./Images/PCB-3D-2.png)

- 使用 **USB Type-C** 接口以及贴片晶振；
- 采用 `STM32F103C8T6` 微控制器方案；
- 低压差线性稳压器 **LDO** 调整为 `ME6211C33M5G` 方案；
- 兼容 [ARMmbed DAPLink](https://github.com/ARMmbed/DAPLink/releases/tag/v0257) 提供的 `REL v0257` 最新版固件；
- 提供 **SWD/JTAG** 转换板，以及清晰的符号标识；
- 预留 `1mm` 和 `2mm` 直径固定螺丝孔，方便与外壳进行固定；

# UINIO-DAP-Link 下载调试器

[**UINIO-DAP-Link**](https://github.com/uinika/UINIO-DAP-Link) 是一款基于 [**ARM DAP Link**](https://daplink.io/) 开源固件的硬件下载调试电路设计，采用了 `LQFP48` 封装的 **STM32F103CBT6** 或者 **STM32F103C8T6** 微控制器作为主控芯片，同时也兼容其它 `Pin to Pin` 的 **Cortex-M3** 微控制器（需要自行调整固件）。

![](./Images/PCB-3D-1.png)

![](./Images/PCB-3D-2.png)

- 采用 **USB Type-C** 接口以及 **3225** 封装的贴片晶振；
- 提供 **SWD/JTAG** 转换板，以及清晰合理的符号标识；
- 低压差线性稳压器 **LDO** 调整为 `ME6211C33M5G` 方案；
- 兼容 [ARMmbed DAPLink](https://github.com/ARMmbed/DAPLink/releases/tag/v0257) 提供的 `REL v0257` 最新版本固件；
- 预留 `1mm` 和 `2mm` 直径固定螺丝孔，方便与外壳进行固定；
- 工程中的 `Firmware` 目录提供了已经编译好的最新版 DAPLink 0258 固件的 Bootloader 以及 Interface；
- 更多关于 UINIO-DAP-Link 在 STM32CubeIDE 以及 Keil µVision 当中的应用，以及固件下载升级方法，请参见 [ARM 调试工具 UINIO-DAP-Link 应用指南](http://uinio.com/Project/UINIO-DAP-Link/)；
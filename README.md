# UINIO-DAP-Link 下载调试器

[**UINIO-DAP-Link**](https://gitee.com/uinika/UINIO-DAP-Link) 是一款基于 [**ARM DAP Link**](https://daplink.io/) 开源固件的硬件下载调试电路设计，采用了 `LQFP48` 封装的 **STM32F103CBT6** 或者 **STM32F103C8T6** 微控制器作为主控芯片，同时也兼容其它 `Pin to Pin` 的 **Cortex-M3** 微控制器（需要自行调整固件）。

![](./Images/PCB-3D-1.png)

![](./Images/PCB-3D-2.png)

## 设计概要

1. 采用 **USB Type-C** 接口以及 **3225** 封装的贴片晶振；
2. 提供 **SWD/JTAG** 转换板，以及清晰合理的符号标识；
3. 低压差线性稳压器 **LDO** 调整为 `ME6211C33M5G` 方案；
4. 兼容 [ARMmbed DAPLink](https://github.com/ARMmbed/DAPLink/releases/tag/v0257) 提供的 `REL v0257` 最新版本固件；
5. 预留 `1mm` 和 `2mm` 直径固定螺丝孔，方便与外壳进行固定；
6. 工程中的 `Firmware` 目录提供有已编译的最新 **DAPLink 0258** 版本固件的 `Bootloader` 以及 `Interface`；

## 参考技术文档

[UinIO.com 电子技术实验室](http://uinio.com/) 为 UINIO-DAP-Link 开源项目提供了如下一系列技术参考资料：

- [**《ARM 调试工具 UINIO-DAP-Link 应用指南》**](http://uinio.com/Project/UINIO-DAP-Link/)：介绍 UINIO-DAP-Link 在 **STM32CubeIDE** 以及 **Keil µVision** 开发环境当中的使用，以及 DAPLink 固件的下载更新方法。
- [**《BOM 交互式物料清单与 PCB 布线在线预览》**](http://uinio.com/archives/BOM/UINIO-DAP-Link.html)：介绍了 UINIO-DAP-Link 硬件 PCB 所涉及的物料清单与布线预览。

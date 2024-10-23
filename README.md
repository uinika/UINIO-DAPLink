# UINIO-DAP-Link 下载调试器

[**UINIO-DAP-Link**](https://gitee.com/uinika/UINIO-DAP-Link) 是一款基于 [**ARM DAP Link**](https://daplink.io/) 开源固件的硬件下载调试电路设计，采用了 `LQFP48` 封装的 **STM32F103CBT6** 或者 **STM32F103C8T6** 微控制器作为主控芯片，同时也兼容其它 `Pin to Pin` 的 **Cortex-M3** 微控制器（需要自行调整固件）。

https://github.com/ARMmbed/mbed-HDK-Eagle-Projects

![](./Images/PCB-3D-1.png)

![](./Images/PCB-3D-2.png)

## 设计概要

1. 清晰合理的丝印标识，并且预留有 `2mm` 直径的固定螺丝孔；
2. **USB Type-C** 接口位置新增一组 TVS 瞬态电压抑制二极管；
3. 专门为 `5V` 引脚接口添加了保险丝与二极管组成的防反接电路；
4. 附带有 **SWD** 和 **JTAG** 协议的转接板，以及相关功能的跳线位；
5. 低压差线性稳压器 **LDO** 调整为南京微盟电子的 `ME6211C33M5G` 方案；
6. 工程的 `Firmware` 目录已经编译好 **DAPLink 0258** 版本固件的 `Bootloader` 以及 `Interface` 二进制文件；
7. 兼容 [ARMmbed DAPLink](https://github.com/ARMmbed/DAPLink/releases/tag/v0257) 提供的 `REL v0257` 最新版本固件；

## 参考技术文档

[UinIO.com 电子技术实验室](http://uinio.com/) 为 UINIO-DAP-Link 开源项目提供了如下一系列技术参考资料：

- [**《ARM 调试工具 UINIO-DAP-Link 应用指南》**](http://uinio.com/Project/UINIO-DAP-Link/)：介绍 UINIO-DAP-Link 在 **STM32CubeIDE** 以及 **Keil µVision** 开发环境当中的使用，以及 DAPLink 固件的下载更新方法。
- [**《BOM 交互式物料清单与 PCB 布线在线预览》**](http://uinio.com/archives/BOM/UINIO-DAP-Link.html)：介绍了 UINIO-DAP-Link 硬件 PCB 所涉及的物料清单，并且还提供了布线的预览。

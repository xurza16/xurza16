<div align="center">

# 杨一帆

**嵌入式软件工程师** ｜ MCU 固件 · FreeRTOS · Bootloader/OTA · 机器人控制 ｜ 深圳

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-000000?style=flat-square)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)

求职：嵌入式软件 / 固件开发 / 机器人控制（深圳）<br>
邮箱：finnyoun9@gmail.com

</div>

## 技术方向

- **MCU 固件** — C、STM32 HAL、FreeRTOS、Bootloader、OTA、UART/I²C/SPI、看门狗
- **机器人控制** — 电机驱动、编码器测速、PID 与运动学、STM32 ↔ 树莓派通信、ROS 2
- **硬件排查** — 板级 bring-up、逻辑分析仪与示波器调试、CI 与 SIL 测试

## 代表项目

| 项目 | 内容 | 验证状态 |
| --- | --- | --- |
| [麦克纳姆轮自主移动机器人](https://github.com/finnyoun9/mecanum-robot) | STM32F103 + FreeRTOS + 树莓派 5 + ROS 2 Jazzy，四轮驱动、自定义串口协议、SLAM 与边缘视觉 | 真机：四电机方向实测通过；固件 SIL 与 ROS 2 构建有 CI |
| [智能家居 OTA 系统](https://github.com/finnyoun9/stm32-smart-home-ota) | STM32F103 + FreeRTOS + ESP32 双核协作，自研 8KB Bootloader、CRC-32 校验、分块确认与重传 | **硬件端到端实测**：PC → 蓝牙 → ESP32 → Bootloader → 写入 Flash → 跳转应用 |
| [FreeRTOS 便携测量仪](https://github.com/finnyoun9/stm32-freertos-instrument) | 示波器 + 数字万用表 + 信号发生器三合一，共用 ADC/DMA/LCD/按键框架 | 内核移植有 ELF 向量表实测；其余条目按「已实测/待实测」逐条标注 |
| [STM32 PID 平衡车](https://github.com/finnyoun9/stm32-pid-balancer) | 串级 PID 自平衡，编码电机速度环与位置环（MIT 许可） | 单电机开环与编码器固件已编译通过，待实物验证 |
| [嵌入式硬件调试工具链](https://github.com/finnyoun9/embedded-debug-toolchain) | 可复用的排查流程：万用表 → 逻辑分析仪 → 示波器 → ST-Link/GDB | 板级 bring-up 与协议诊断的常用参考 |

> 各项目 README 都把**已实测结果**与**设计/进行中**分开写 —— 没验证过的不写成"已完成"。

## 背景

西安交通大学 · 生物医学工程 · 本科（2019–2023）。

曾从事扫地机器人与智能家居产品的技术支援工作，熟悉产品级联调、问题定位与测试闭环。目前专注 MCU 固件与机器人控制方向。

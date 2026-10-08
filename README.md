<div align="center">

# 林子越

**嵌入式软件开发** ｜ MCU 固件 · FreeRTOS · 无人机控制

广东工业大学 · 电子信息工程 · 本科在读（2024–2028）｜ 广州

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-000000?style=flat-square)
![CYT4BB7](https://img.shields.io/badge/CYT4BB7-双核_Cortex--M7-34495E?style=flat-square)
![MSPM0](https://img.shields.io/badge/MSPM0G3507-CC0000?style=flat-square)

求职方向：嵌入式软件工程师<br>
邮箱：[miurczy123@outlook.com](mailto:miurczy123@outlook.com)

</div>

## 技术方向

- **MCU 与外设驱动** — C/C++，STM32、CYT4BB7、TC264、MSPM0G3507；UART、I²C、SPI、PWM、ADC、Timer、DMA
- **实时系统** — FreeRTOS 任务划分与调度，队列、信号量、互斥锁，中断与任务协作，双核 IPC 通信
- **通信设计** — 中断接收与协议解析解耦，FIFO、非阻塞发送队列，CRC16、ACK、序号校验与超时处理
- **控制与状态估计** — 串级 PID、前馈与摩擦补偿，数字滤波、Kalman、Alpha-Beta、TD，多传感器融合
- **开发与调试** — Keil、IAR、ADS、CCS、VS Code，ST-Link、DAP-Link，串口日志、示波器、逻辑分析仪；Git、Markdown

## 代表项目

### 四旋翼自主飞行控制系统

**平台：** CYT4BB7 双 Cortex-M7 · FreeRTOS · IMU · ToF · 光流

负责嵌入式软件与控制算法。按驱动、数据处理和控制应用分层，0 核运行实时飞控任务，1 核承担视觉与辅助计算，通过 IPC 共享数据。

- **多频率实时任务：** 设计传感器采集、状态估计、飞行控制、通信、日志 5 类任务，使用队列和信号量组织 500 Hz IMU/控制、100 Hz 高度估计与 40 Hz XY 状态估计。
- **实时通信：** 将 UART 中断接收、数据搬运、协议解析和业务处理拆分，结合最新状态覆盖、序号校验与超时检测处理无人机和车机之间的状态交互。
- **估计与控制：** 融合 IMU、双 ToF 选源与光流，加入异常检测与补偿，实现 XYZ 状态估计及串级 PID 控制；项目记录的俯仰/横滚精度为 ±2°，平面定位误差小于 5 cm。
- **日志与调参：** 结合上位机多变量日志和 Flash 黑盒记录，通过波形分析检查估计与控制链路，迭代滤波和控制参数。

### 车载平衡滚球运动控制系统

**平台：** MSPM0G3507 · 树莓派视觉 · Emm42 闭环步进电机 · SPI + DMA

负责钢球实时控制。接收视觉位置数据，完成钢球状态估计、位置/速度串级控制和电机执行，控制车辆运动过程中的钢球位置。

- **控制链路：** 使用 Alpha-Beta / TD 平滑视觉位置并估计速度，构建位置外环与速度内环；加入车体加速度前馈、静摩擦补偿、限幅和视觉失效保护。
- **电机驱动：** 封装 Emm42 串口驱动，通过非阻塞发送队列与多类型应答解析实现绝对位置控制。
- **显示优化：** 将 TFT 同步 SPI 刷新改为 SPI + DMA 异步传输，降低显示任务对实时控制的阻塞。

## 教育与荣誉

**广东工业大学 · 电子信息工程 · 本科在读（2024–2028）**

GPA：3.60 / 5.00 ｜ CET-6：575<br>
相关课程：信号与系统、模拟电子技术、数字电子技术、微机原理与接口技术、C 语言程序设计

- **2026** — 广东工业大学优秀学生奖学金二等奖
- **2026** — 全国大学生智能汽车竞赛华南赛区二等奖
- **2026** — 全国大学生嵌入式芯片与系统设计竞赛南部赛区二等奖
- **2026** — 全国大学生电子设计竞赛广东省三等奖
- **2025** — 蓝桥杯全国软件和信息技术专业人才大赛广东省二等奖

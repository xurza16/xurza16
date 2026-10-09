<div align="center">

# 林子越

**嵌入式开发 · 状态估计 · 运动控制**

广东工业大学 · 电子信息工程 · 2024–2028

[![GitHub](https://img.shields.io/badge/GitHub-xurza16-181717?style=flat-square&logo=github)](https://github.com/xurza16)
[![Email](https://img.shields.io/badge/Email-Outlook-0078D4?style=flat-square)](mailto:miurczy123@outlook.com)

</div>

用 C 做 MCU 开发，实践集中在传感器采集、设备通信和闭环控制。这里记录我做过的项目，以及从驱动、状态估计到执行机构的实现过程。

## 🏆 个人荣誉

| 年份 | 荣誉 |
| :---: | --- |
| 2026 | 全国大学生智能汽车竞赛 · 华南赛区二等奖 |
| 2026 | 全国大学生嵌入式芯片与系统设计竞赛 · 南部赛区二等奖 |
| 2026 | 全国大学生电子设计竞赛 · 广东省三等奖 |
| 2026 | 广东工业大学优秀学生奖学金 · 二等奖 |
| 2025 | 蓝桥杯全国软件和信息技术专业人才大赛 · 广东省二等奖 |

## 🛠️ 技术栈

| 功能方向 | 技术与实践 |
| --- | --- |
| **语言与平台** | C / C++ · STM32 · CYT4BB7 · TC264 · MSPM0G3507 |
| **实时调度与核间协作** | 裸机定时器调度 · FreeRTOS · 中断与任务协作 · 队列 / 信号量 / 互斥锁 · 双核 IPC |
| **外设与数据采集** | UART · I²C · SPI · PWM · ADC · Timer · DMA · 传感器驱动 |
| **通信与协议** | FIFO · 非阻塞收发 · CRC16 · ACK · 序号校验 · 超时处理 |
| **状态估计与滤波** | IMU / ToF / 光流融合 · Kalman · Alpha-Beta · TD · 数字滤波 |
| **运动控制** | 串级 PID · 前馈补偿 · 摩擦补偿 · 执行器限幅与失效保护 |
| **开发与调试** | IAR · Keil · CCS · ADS · VS Code · Git · 串口日志 · 示波器 · 逻辑分析仪 |

## 🚀 项目

| 项目 | 主要实践 | 
| --- | --- | 
| **[F5 · 四旋翼飞控软件](https://github.com/xurza16/F5)** | CYT4BB7 双核飞控与视觉处理；IMU、双 ToF、光流状态估计；串级 PID、IPC 与设备通信 |
| **车载平衡滚球运动控制系统** | MSPM0G3507 + 树莓派视觉；钢球位置 / 速度控制、Emm42 驱动、SPI + DMA 显示 |

---

📬 [miurczy123@outlook.com](mailto:miurczy123@outlook.com) · [所有仓库](https://github.com/xurza16?tab=repositories)

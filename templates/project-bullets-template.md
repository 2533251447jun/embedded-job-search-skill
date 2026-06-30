# Project Bullets Template

Use this template to extract resume-safe embedded project bullets from real evidence. Fields may be left blank, marked `needs_proof`, or removed when not applicable. Do not invent project duration, team size, enterprise background, customer delivery, mass production, or performance metrics.

## 基本信息

- 项目名称：
- 项目性质：课程 / 实训 / 毕设 / 实验室 / 个人 / 实习 / 企业
- 目标岗位族：STM32/MCU 固件 / 嵌入式测试 / 硬件联调 / IoT / 工业控制 / BSP/Linux 初级 / 车载测试
- JD 对应关键词：
- 项目来源：
- 开发周期：可留空；无证据时标 `needs_proof`
- 团队规模：可留空；无证据时不得编造人数
- 个人角色：独立完成 / 参与完成 / 协助完成 / 学习内容 / 阅读内容 / 跑通 demo / 修改示例代码

## 可提供证据

| 证据类型 | 是否可提供 | 说明 |
|---|---|---|
| 代码 / Git Commit |  |  |
| 实验/课程/项目报告 |  |  |
| 图片 / 视频 |  |  |
| 调试日志 / 串口日志 |  |  |
| 波形截图 |  |  |
| 测试报告 |  |  |
| 调试记录 |  |  |

## 技术平台

- MCU：STM32 / GD32 / ESP32 / NXP / TI / Nordic / AVR / 8051 / 其他
- 开发板：
- 开发环境：Keil / MDK、STM32CubeIDE、IAR、VS Code
- 编译工具：GCC、ARMCC、Clang、其他
- 版本管理：Git / SVN / 无
- 操作系统：Bare Metal / 裸机、FreeRTOS、RT-Thread、Linux
- 深度边界：L1 知道是什么 / L2 能够使用 / L3 能够调试 / L4 能够分析问题 / L5 能够设计
- 如果只是学习过或跑过 demo：写“学习中 / demo / needs_proof”，不得写成项目经验。

## 外设与通信

| 外设/协议 | 真实使用场景 | 是否调试过问题 | 证据 | 可写边界 | 不允许夸大 |
|---|---|---|---|---|---|
| GPIO / EXTI |  |  |  |  | 不写成完整驱动框架 |
| UART / USART / TTL / RS232 |  |  |  |  | 不写成协议栈设计 |
| RS485 / Modbus RTU / Modbus TCP |  |  |  |  | 不写成工业通信平台负责人 |
| I2C / SPI / QSPI |  |  |  |  | 不写成高速总线专家 |
| CAN / CAN FD |  |  |  |  | 无工具证据不写 CANoe/CANalyzer |
| ADC / DAC / PWM / TIM / DMA |  |  |  |  | 无实测数据不写性能优化 |
| RTC / Flash / EEPROM / SDIO / FatFS |  |  |  |  | 不写成可靠存储方案设计 |
| MQTT / HTTP / BLE / Wi-Fi / LoRa |  |  |  |  | 无项目证据不写 IoT 落地 |

## 项目目标

- 业务目标：可留空；无真实背景时不要编造。
- 功能目标：
- 技术目标：
- 学习目标：
- 性能目标：无实测数据时标 `needs_proof` 或写“未量化”。

## 个人职责边界

- `fact`：我实际完成的功能、调试、测试或文档。
- `inference`：基于事实可合理推断的能力。
- `needs_proof`：证据不足，不能直接写进简历。
- `not_allowed`：用户要求编造、夸大、伪造或绕过平台规则。
- 他人/团队/教程完成的部分：
- 只阅读、学习、跑 demo 或修改示例代码的部分：

## 实际完成内容

| 类型 | 内容 | 标签 | 证据 |
|---|---|---|---|
| 完成模块 |  | `fact` / `inference` / `needs_proof` |  |
| 新增功能 |  |  |  |
| Bug 修复 |  |  |  |
| 联调内容 |  |  |  |
| 测试内容 |  |  |  |
| 参数配置 / 日志整理 / 代码整理 |  |  |  |

## 调试过程

- 发现问题：
- 复现方式：
- 定位过程：
- 排查路径：
- 使用工具：万用表 / multimeter、示波器 / oscilloscope、逻辑分析仪 / logic analyzer、串口助手 / serial terminal
- 关键证据：
- 修复方案：
- 验证过程：
- 遗留问题：

## Bug / 异常记录

- 问题编号：
- 问题描述：
- 影响范围：
- 复现方式：
- 原因分析：
- 修复方案：
- 验证结果：
- 是否再次出现：
- 是否有日志 / 截图 / 波形 / Git Commit：

## 验证方式

可选：串口日志、波形、寄存器、示波器、逻辑分析仪、万用表、截图、测试报告、视频、Git Commit、课程报告、实验报告。

没有验证方式时，不得写“验证通过”“稳定运行”“长期可靠”。

## Evidence

- `evidence_status`：`verified` / `partially_verified` / `user_claimed` / `needs_proof` / `not_allowed`
- 证据来源：
- 证据充分度：★★★★★ / ★★★★☆ / ★★★☆☆ / ★★☆☆☆ / ★☆☆☆☆
- 仍缺少的证据：
- 是否可直接写入简历：YES / NO / needs_proof
- 是否需要降级表达：

## 简历 Bullet 输出

### 正式版

- Bullet：
- 可写强度：强 / 中 / 弱 / 不可写
- 证据状态：
- 面试风险：
- 是否需要 `needs_proof`：

### 保守版

- Bullet：
- 适用场景：
- 降级原因：

### 技术版

- Bullet：
- ATS 关键词：

### HR 版

- Bullet：
- 避免过度技术化的解释：

### 英文版（可选）

- Bullet：

## 面试准备

- 高频追问：
- 容易问倒的问题：
- 不能回答的内容：
- 建议降级表达：
- 可引用证据：
- 不能引用内容：
- 如果答不上，应如何诚实说明：

## 禁止表达

无强证据时不得写：

- 主导整个系统
- 负责全部固件
- 独立完成 BSP
- 量产负责人
- 架构设计者
- 企业核心成员
- 客户现场负责人
- 百万级设备部署
- 完整协议栈设计
- 负责平台化建设

若无法提供证据，标记 `needs_proof`；若用户要求编造，标记 `not_allowed`。

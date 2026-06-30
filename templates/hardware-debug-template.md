# Hardware Debug Template

Use this as an embedded joint-debug record, not a generic problem-solution note. Leave unknown fields blank or mark `needs_proof`. Do not write instrument or field-debug experience that the candidate cannot explain.

## 调试案例基础信息

- 问题标题：
- 问题分类：软件 / 驱动 / 协议 / 硬件 / 供电 / PCB / EMC-ESD / 环境 / 工具 / 人为配置
- 发现阶段：开发 / 联调 / 测试 / 复测 / 面试复盘
- 软件版本：可留空；无证据时标 `needs_proof`
- 硬件版本：可留空；无证据时标 `needs_proof`
- MCU 平台：
- 外设：
- 通信接口：
- 调试环境：
- `evidence_status`：

## 场景覆盖清单

| 场景 | 现象 | 初步怀疑 | 关键工具 | 关键证据 | 不允许夸大 |
|---|---|---|---|---|---|
| 串口无输出 |  | TX/RX、波特率、时钟、复位 | 串口助手 / serial terminal、万用表 / multimeter | 日志、电压、接线 | 不写成通信协议专家 |
| I2C 无 ACK |  | 地址、上拉、电平、复用配置 | 逻辑分析仪 / logic analyzer、示波器 / oscilloscope | 波形、地址扫描、代码 | 没用过仪器不得写熟练使用 |
| SPI 时序异常 |  | CPOL/CPHA、片选、线序 | 逻辑分析仪、示波器 | 时序图、寄存器配置 | 不写成高速总线设计 |
| ADC 读数漂移 |  | 参考电压、采样时间、接地 | 万用表、示波器 | 电压读数、采样日志 | 无实测不写精度优化 |
| PWM 无输出 |  | 定时器、GPIO 复用、占空比 | 示波器、代码断点 | 波形、寄存器 | 不写成电机控制专家 |
| 中断不触发 |  | NVIC、优先级、标志位 | Debugger、寄存器窗口 | 中断标志、断点 | 不写成实时系统设计 |
| 下载失败 / 复位异常 |  | BOOT0、NRST、SWD、供电 | ST-Link/J-Link、万用表 | 下载日志、电压 | 不写成板级 bring-up 负责人 |
| 供电 / 接地 / 接线问题 |  | 电源、GND、杜邦线、焊点 | 万用表、可调电源 / bench power supply | 电压、连线照片 | 只会接线不得写硬件设计 |
| BOOT0 / NRST / SWD 问题 |  | 启动模式、复位、电平 | ST-Link/J-Link、万用表 | 电平、下载日志 | 不写成底层启动专家 |
| 晶振问题 |  | 晶振不起振、PLL 配置 | 示波器、寄存器 | 时钟波形、配置 | 不写成硬件设计经验 |

## 复现与现象

- 复现条件：
- 现象描述：
- 错误日志：
- 波形/读数：
- 影响范围：
- 是否可稳定复现：

## 调试知识树

按顺序排查并记录证据：

1. 软件问题：
2. 驱动问题：
3. 协议问题：
4. 硬件问题：
5. 供电问题：
6. PCB 问题：
7. EMC / ESD 问题：
8. 环境问题：
9. 工具问题：
10. 人为配置问题：

## 排查步骤

| 步骤 | 操作 | 使用工具 | 观察结果 | 结论 | 标签 |
|---|---|---|---|---|---|
| 1 |  |  |  |  | `fact` / `inference` / `needs_proof` |
| 2 |  |  |  |  |  |
| 3 |  |  |  |  |  |

## 使用工具与证据

- 万用表 / multimeter：供电、GND、IO 电平、连通性。
- 示波器 / oscilloscope：波形、时钟、PWM、毛刺、边沿。
- 逻辑分析仪 / logic analyzer：I2C/SPI/UART/RS485 时序和协议帧。
- 串口助手 / serial terminal：日志、收发、波特率验证。
- Debugger：断点、寄存器、内存、调用栈、HardFault。
- 关键证据：波形 / 日志 / 电压 / 寄存器 / 连线 / 截图 / Git Commit。

## 根因与修复

- 根因分析：
- 修复方式：
- 验证方式：
- 复测结果：
- 遗留风险：

## 简历可写表达

- 可写入版本：
- 降级版本：
- 可写强度：强 / 中 / 弱 / 不可写
- `evidence_status`：
- `needs_proof`：

## 面试追问

- 你为什么先查供电/接地？
- 示波器或逻辑分析仪如何连接？
- 如何确认 I2C 地址、上拉和 ACK？
- 如何确认 SPI CPOL/CPHA？
- 如何判断 ADC 漂移是硬件还是软件问题？
- 下载失败如何定位 BOOT0/NRST/SWD？
- 如果没有使用过某个工具，如何诚实说明？

## 不允许夸大的表达

- 没有用过示波器，不得写“熟练使用示波器”。
- 只会接线，不得写“硬件设计”。
- 只会看串口日志，不得写“通信协议专家”。
- 只排查过开发板问题，不得写“现场调试负责人”。

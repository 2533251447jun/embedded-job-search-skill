# Embedded Role Keywords

Each keyword should be treated as a routing signal, not as permission to add the skill to a resume. Evidence decides wording.

| Role family | Keywords | Junior fit | Evidence needed | Downgrade if no proof |
|---|---|---|---|---|
| STM32/MCU firmware | STM32, GD32, ESP32, 51, MCU, HAL, LL, CubeMX, Keil, GPIO, UART, I2C, SPI, ADC, TIM, PWM, DMA, Flash, RTC, Watchdog | High | Code, board, peripheral behavior, logs, debug notes | “完成基础外设配置/学习中” |
| Embedded testing | 测试用例, 测试计划, 缺陷复现, 回归测试, 长稳测试, 串口日志, 波形, 测试报告, Unity, Ceedling | High | Test cases, report, issue records, logs, waveforms | “参与功能验证/整理日志” |
| Hardware debug/joint debug | 硬件调试, 联调, 万用表, 示波器, 逻辑分析仪, 串口助手, I2C 无 ACK, ADC 漂移, 下载失败 | High | Instrument use, wiring, schematic notes, fault reproduction | “配合联调/学习仪器使用” |
| IoT device side | IoT, ESP32, Wi-Fi, BLE, MQTT, HTTP, CoAP, NB-IoT, 4G Cat.1, OTA, FOTA, 断线重连, 心跳包 | Medium | Connection logs, topics, reconnect behavior, device state, power data | “了解联网流程/完成基础接入” |
| Industrial control/data acquisition | RS485, Modbus RTU, Modbus TCP, CAN, CRC, 轮询, 采集周期, 工业网关, 故障记录 | High | Frame logs, CRC handling, multi-device polling, long-run records | “学习协议帧/完成单设备验证” |
| BSP/driver/Linux | BSP, Linux, U-Boot, Kernel, Device Tree, Kconfig, Makefile, Buildroot, Yocto, dmesg, sysfs | Medium | Device tree snippet, boot log, driver verification, board notes | “了解 BSP/Linux 基础” |
| Vehicle embedded testing | CAN, UDS, DBC, CANoe, CANalyzer, HIL, SIL, ASPICE, ISO 26262, 需求追踪 | Medium to low for entry-level | Tool screenshots, test cases, bus logs, defect records | “了解车载测试流程/无平台实操” |
| Medical/instrument/security/access/consumer | 医疗设备, 仪器仪表, 门禁, 安防, 智能锁, 小家电, OLED, LCD, RTC, 可靠性, 老化测试 | High | Device function, state machine, boundary tests, reliability notes | “完成基础功能验证” |
| Entry-level role | 助理, 初级, 应届, 实习, 培训, 课程设计, 实训, 个人项目 | High | Clear project nature and personal responsibility | “按初级定位表达” |
| High-risk exaggeration | 精通, 主导, 量产, 客户交付, 两年经验, 架构设计, 协议栈, 车规, 功能安全, 医疗认证 | Low without proof | Strong artifacts and interviewer-ready details | Mark `needs_proof` or `not_allowed` |

## Routing Notes

- A JD mentioning “STM32 + RS485 + Modbus” usually routes to MCU firmware plus industrial control.
- A JD mentioning “测试用例 + 串口日志 + CANoe” routes to embedded testing or vehicle communication testing, not firmware development.
- A JD mentioning “Device Tree + dmesg + sysfs” routes to BSP/Linux even if it also mentions C.
- A JD mentioning “示波器 + I2C 无 ACK + 供电” routes to hardware debug/joint debug.

## Chinese/English Keyword Mapping

| 方向 | 中文关键词 | English / ATS keywords | JD 常见表达 | 初级可写表达 | 需要证据 | 无证据降级 | 不允许夸大 |
|---|---|---|---|---|---|---|---|
| STM32 / MCU 固件 | 单片机、外设驱动、串口、中断、定时器 | STM32, MCU, HAL, GPIO, UART, ADC, DMA, TIM | 熟悉 STM32、会 C、能调外设 | 基于 STM32 完成基础外设配置与数据采集 | 代码、工程截图、调试日志、板卡运行结果 | 学习过 STM32 基础外设配置 | 精通底层架构、主导量产固件 |
| 嵌入式测试 | 测试用例、串口日志、缺陷复现、回归测试 | embedded testing, test case, serial log, bug reproduction, regression | 编写测试用例、输出测试报告 | 参与功能验证，整理日志和复现步骤 | 测试记录、日志、报告、缺陷单 | 参与基础功能验证 | 负责完整测试体系 |
| 硬件调试 / 联调 | 供电、接线、示波器、逻辑分析仪、I2C 无 ACK | hardware debug, joint debug, oscilloscope, logic analyzer | 能配合硬件调试 | 配合检查供电、接线、波形或日志 | 波形、电压、接线图、排查记录 | 配合联调，学习仪器使用 | 精通硬件设计、现场负责人 |
| IoT | 物联网、MQTT、联网、心跳、断线重连 | IoT, MQTT, Wi-Fi, BLE, heartbeat, reconnect | 设备接入云平台 | 完成基础联网和状态上报 demo | 设备日志、topic、联网记录 | 了解联网流程 | 云平台负责人、OTA 落地 |
| 工业控制 / RS485 / Modbus | 工控、RS485、Modbus、CRC、轮询 | industrial control, RS485, Modbus RTU, CRC, polling | 熟悉 Modbus 通信 | 完成基础 Modbus RTU 帧收发和 CRC 校验 | 协议帧、串口日志、代码、调试记录 | 学习协议帧，完成单设备验证 | 主导工业协议栈或客户交付 |
| BSP / Linux 初级 | 设备树、驱动、交叉编译、dmesg | BSP, Linux driver, Device Tree, cross-compilation, dmesg | 了解 Linux 驱动 | 了解 Device Tree、dmesg 和 sysfs 验证流程 | DTS、启动日志、驱动实验记录 | 了解 BSP/Linux 基础 | 驱动专家、bring-up 负责人 |
| 车载测试 / CAN / UDS | CAN、UDS、DBC、HIL、CANoe | CAN, UDS, DBC, HIL, CANoe, CANalyzer | 车载通信测试 | 了解 CAN/UDS 基础和测试流程 | 工具截图、报文日志、测试用例 | 了解车载测试流程 | 无工具证据写 HIL/CANoe 经验 |
| 医疗 / 仪器 / 安防 / 门禁 / 消费电子 | 仪器仪表、门禁、智能锁、显示、按键 | instrument, access control, smart lock, display, keypad | 设备固件开发 | 完成基础人机交互或传感器采集功能 | 代码、照片、测试记录 | 完成基础功能验证 | 医疗认证、可靠性负责人 |

# Resume Project Example

All entries below are **Example Candidate / Example Project** material for teaching and template testing. They are not real enterprise, customer, mass-production, or commercial delivery claims.

## 示例项目 1：STM32 + RS485 + Modbus 工控数据采集

### 示例背景

- 项目性质：课程 / 个人扩展项目。
- 项目来源：示例项目，不代表真实企业项目。
- 投递岗位：STM32/MCU 初级固件、工业控制 / RS485 / Modbus 初级岗位。
- 候选人真实边界：完成基础主站轮询 demo 和日志记录；未参与工业现场、PLC 系统、客户交付或量产。

### 技术栈

- MCU：STM32F103。
- 开发环境：Keil / MDK、STM32CubeMX。
- 通信接口：UART + RS485 模块 / MAX485。
- 协议：Modbus RTU 基础读寄存器。
- 调试工具：串口助手 / serial terminal、万用表 / multimeter。
- 深度：L2 能够使用，部分 L3 能够调试。

### Evidence

- `fact`: 配置 UART 收发、RS485 方向控制 GPIO、基础 Modbus RTU 查询帧。
- `fact`: 记录串口日志和 CRC 校验结果。
- `inference`: 具备基础工业通信项目表达素材。
- `needs_proof`: 多设备轮询、长稳测试、现场抗干扰、PLC 联调、量产部署。
- `evidence_status`: `partially_verified`，需代码、协议帧截图和调试记录支撑。

### 真实性评分

- 真实性：★★★★☆
- 证据充分度：★★★☆☆
- 夸大风险：★★☆☆☆
- 推荐写入简历：YES, if logs/code exist
- 推荐面试使用：YES, with project boundary explained

### 可写入简历 bullet

- 正式版：基于 STM32F103 实现 UART + RS485 基础通信 demo，完成 Modbus RTU 读寄存器查询帧、CRC 校验和串口日志记录，用于验证主站轮询流程。
- 保守版：完成 STM32 串口收发与 Modbus RTU 基础帧学习 demo，能够说明 CRC 校验、超时和日志排查思路。
- ATS 关键词：STM32, UART, RS485, Modbus RTU, CRC, polling, serial log.

### 不允许写的夸大 bullet

- `not_allowed`: 主导工业控制系统开发并完成客户现场交付。
- `not_allowed`: 负责完整 Modbus 协议栈设计和量产部署。

### 面试追问

- Modbus RTU 帧格式是什么？
- CRC16 如何计算和验证？
- RS485 方向控制如何处理？
- 超时无响应时怎么记录？
- 你是否做过真实 PLC 联调或工业现场测试？

### 答不上时如何降级

如果答不上现场、抗干扰或 PLC 问题，应说明：“该项目是课程/个人 demo，主要验证基础帧收发和 CRC，工业现场联调经验仍在补充。”

## 示例项目 2：嵌入式测试 + 串口日志 + 缺陷复现

### 示例背景

- 项目性质：实验室 / 课程测试任务。
- 项目来源：示例项目，不代表真实公司测试流程。
- 投递岗位：嵌入式测试工程师、嵌入式系统测试助理。
- 候选人真实边界：整理测试用例、串口日志和复现步骤；未负责完整质量体系或自动化测试平台。

### 技术栈

- 被测对象：STM32 传感器采集 demo。
- 工具：串口助手 / serial terminal、Excel/Markdown 测试记录、Git。
- 测试类型：功能测试、边界值测试、回归测试。
- 深度：L2 能够使用，L3 能够复现和辅助定位。

### Evidence

- `fact`: 记录串口日志，复现异常输入导致的显示错误。
- `fact`: 整理测试用例、复测结果和缺陷说明。
- `inference`: 适合表达嵌入式测试入门经验。
- `needs_proof`: 自动化测试、HIL/SIL、系统级覆盖率、质量体系经验。
- `evidence_status`: `partially_verified`，需测试记录、日志和复测截图。

### 真实性评分

- 真实性：★★★★☆
- 证据充分度：★★★★☆
- 夸大风险：★★☆☆☆
- 推荐写入简历：YES
- 推荐面试使用：YES

### 可写入简历 bullet

- 正式版：围绕 STM32 传感器采集 demo 设计基础功能和边界值测试用例，使用串口日志复现异常显示问题，并整理复测记录。
- 保守版：参与嵌入式 demo 功能验证，记录串口日志和异常复现步骤，具备测试记录意识。
- ATS 关键词：embedded testing, serial log, bug reproduction, regression test, test case.

### 不允许写的夸大 bullet

- `not_allowed`: 负责完整嵌入式测试体系建设。
- `not_allowed`: 主导 HIL/SIL 平台测试。
- `not_allowed`: 完成系统级质量覆盖率评估。

### 面试追问

- 测试用例如何设计？
- 异常如何复现？
- 日志里哪个字段说明问题存在？
- 修复后如何回归？
- 没有正式测试报告时，你能提供什么证据？

### 答不上时如何降级

如果答不上自动化或 HIL/SIL，应说明：“目前主要是手工功能测试和日志复现，自动化和 HIL/SIL 只是学习方向。”

## 示例项目 3：硬件联调 + I2C 无 ACK / 串口无输出排查

### 示例背景

- 项目性质：课程 / 实训联调记录。
- 项目来源：示例项目，不代表企业现场调试。
- 投递岗位：硬件调试助理、软硬件联调助理、初级嵌入式测试。
- 候选人真实边界：参与基础排查和记录；未进行 PCB 设计、EMC 设计或现场负责人工作。

### 技术栈

- MCU：STM32F103。
- 外设：I2C OLED、UART。
- 工具：万用表 / multimeter、串口助手 / serial terminal；示波器 / oscilloscope 与逻辑分析仪 / logic analyzer 需有真实使用证据才写。
- 深度：L2 能够使用，部分 L3 能够调试。

### Evidence

- `fact`: 检查 TX/RX 接线、波特率、I2C 地址和上拉电阻。
- `fact`: 用串口助手确认无输出现象，用万用表检查供电和 IO 电平。
- `inference`: 具备基础硬件联调记录能力。
- `needs_proof`: 示波器波形、逻辑分析仪抓包、PCB 级问题、EMC/ESD。
- `evidence_status`: `user_claimed` or `partially_verified`, depending on photos/logs.

### 真实性评分

- 真实性：★★★☆☆
- 证据充分度：★★★☆☆
- 夸大风险：★★★☆☆
- 推荐写入简历：YES, conservative wording only
- 推荐面试使用：YES, if candidate can explain steps

### 可写入简历 bullet

- 正式版：参与 STM32 外设联调，针对 I2C 无 ACK 和串口无输出问题，按供电、电平、接线、地址和波特率顺序完成基础排查并记录复现步骤。
- 保守版：具备基础软硬件联调意识，能够配合检查供电、接线、串口参数和 I2C 地址配置。
- ATS 关键词：hardware debug, I2C ACK, UART, serial terminal, multimeter, joint debug.

### 不允许写的夸大 bullet

- `not_allowed`: 精通硬件设计和 PCB Layout。
- `not_allowed`: 熟练使用示波器和逻辑分析仪完成复杂协议分析，除非有真实波形证据。
- `not_allowed`: 负责客户现场硬件调试。

### 面试追问

- I2C 无 ACK 可能有哪些原因？
- 如何检查上拉电阻和电平？
- 串口无输出先查接线还是波特率？
- BOOT0 / NRST / SWD 与下载失败有什么关系？
- 如果没有示波器经验，如何诚实说明？

### 答不上时如何降级

如果答不上波形或 PCB 问题，应说明：“我参与过基础联调和现象记录，示波器/逻辑分析仪分析仍需补充真实练习。”

---
name: embedded-job-search-skill
description: Use when helping candidates with embedded job search, JD analysis, resumes, project evidence, interview prep, and applications for STM32, MCU, RTOS, hardware debugging, embedded testing, IoT, industrial control, BSP, Linux drivers, and junior firmware roles.
---

# embedded-job-search-skill

## Overview

这是面向中国国内嵌入式相关岗位的求职 Skill Router。核心原则：先判断岗位族，再核验证据，最后生成简历、JD 分析、面试追问或投递沟通文本。

不要把它当作泛求职 Skill。所有输出必须围绕嵌入式项目证据、硬件/固件/测试/IoT/工控/BSP/Linux 路由和反夸大边界。

## When to Use

- 用户要分析 STM32、MCU、RTOS、嵌入式测试、硬件调试、IoT、工控、BSP、Linux 驱动、车载通信测试等岗位。
- 用户要把课程、实训、个人项目、实习项目整理成嵌入式简历项目。
- 用户要准备 UART、I2C、SPI、ADC、DMA、FreeRTOS、RS485/Modbus、CAN、MQTT、硬件联调等面试追问。
- 用户要生成 Boss 直聘、邮件、HR 跟进、面试后跟进等投递沟通文本。

## When Not to Use

- 纯互联网、产品、运营、设计、非嵌入式通用求职任务。
- 用户要求伪造学历、实习、企业项目、量产、客户交付、上线、薪资、证书或年限。
- 用户要求自动投递、自动私信、绕过招聘平台限制或批量骚扰 HR。
- 用户只需要法律、移民、财务或医疗职业建议。

## Supported Role Families

先把任务路由到一个或多个岗位族：

| 岗位族 | 典型信号 | 优先证据 |
|---|---|---|
| STM32/MCU 固件 | STM32、GD32、ESP32、51、HAL、外设驱动 | 代码、板卡、外设、调试日志、功能验证 |
| 嵌入式测试 | 测试用例、缺陷复现、回归、长稳、HIL/SIL | 测试报告、日志、波形、缺陷记录 |
| 硬件调试/联调 | 串口无输出、I2C 无 ACK、ADC 漂移、下载失败 | 接线、原理图、仪器截图、排查路径 |
| IoT 设备端 | Wi-Fi、BLE、MQTT、HTTP、OTA、低功耗 | 联网流程、topic、日志、异常恢复 |
| 工业控制/采集 | RS485、Modbus、CAN、采集周期、CRC | 协议帧、轮询、故障日志、长稳记录 |
| BSP/驱动/Linux | Device Tree、U-Boot、Kernel、dmesg、sysfs | 设备树片段、驱动验证、bring-up 记录 |
| 车载通信测试 | CAN、UDS、DBC、CANoe、HIL、ASPICE | 工具使用、测试用例、报文分析、缺陷闭环 |
| 医疗/仪器/安防/门禁/消费电子 | 传感器、显示、按键、RTC、可靠性 | 设备状态机、边界测试、异常记录 |

详见 `references/embedded-role-keywords.md`。

## Candidate Level Routing

- 应届/初级：强调真实项目细节、可追问点、调试过程和学习边界。
- 转嵌入式：把原专业/经验映射到嵌入式证据，不虚构企业项目。
- 课程/实训项目：必须保留项目性质，不能写成公司、客户或量产项目。
- 少量实习经验：区分个人职责、团队职责、公司已有框架和个人实际产出。

## Intake Questions

开始输出前，优先补齐：

1. 目标城市、岗位族、行业方向和候选人级别。
2. 项目性质：课程、实训、个人、实习、企业。
3. 芯片/板卡、开发环境、外设、协议、RTOS、调试工具。
4. 证据：代码、照片、日志、波形、测试报告、仓库、演示视频。
5. 边界：哪些只是看过教程、了解概念、由别人完成、没有报告或没有代码。

## JD Deep-Dive Workflow

1. 提取 JD 中的芯片、协议、工具、行业、职责和隐含门槛。
2. 判断岗位族，不确定时列出候选路由和依据。
3. 区分硬性要求、加分项、隐含要求和高风险追问。
4. 与候选人证据对齐，标出匹配项、短板和 `needs_proof`。
5. 给出投递建议：可投、谨慎投、暂不建议，并说明补证据任务。

## Evidence Chain Rules

所有输出必须使用这些标签：

- `fact`：用户明确提供、简历/JD/文件中明确存在的事实。
- `assumption`：为完成分析临时假设，必须显式标注并可被用户纠正。
- `inference`：基于事实推断出的结论，不能写成事实。
- `user_preference`：用户的城市、薪资、行业、岗位偏好。
- `needs_proof`：证据不足，不能直接写进简历或当作项目经验。

证据状态使用：

- `verified`：有代码、报告、日志、波形、仓库或文件可核对。
- `partially_verified`：只有部分证据，输出要保守。
- `user_claimed`：用户口述但未见证据。
- `needs_proof`：用户说“应该会”“看过”“想写”，但缺少可追问证据。
- `not_allowed`：编造、夸大、自动投递、自动私信、绕过平台规则。

无证据时必须降级表达，例如“了解”“学习中”“接触过概念”“完成基础验证”，不能写“熟练”“精通”“主导”“量产”“客户交付”。

## Resume Optimization Workflow

1. 对每个项目建立证据链：项目性质、芯片、外设、协议、个人职责、调试过程、验证方式。
2. 先写 `fact` 版本，再写简历 bullet。
3. 每条 bullet 后列出证据来源、可追问点、风险等级和是否可直接写入简历。
4. 没有证据的能力进入补证据清单，不进入正式简历。
5. 对课程/实训/个人项目保留真实属性，不能写成企业或量产项目。

## Embedded Project Bullet Patterns

优先使用“场景 + 技术动作 + 调试/验证 + 结果边界”：

- STM32/MCU：芯片、外设、驱动、状态机、中断/DMA/轮询、日志、验证。
- 嵌入式测试：测试目标、用例、日志/波形、缺陷复现、回归验证。
- 工控/Modbus：RS485、帧格式、CRC、轮询、超时、异常恢复、长稳。
- IoT：联网、MQTT topic、断线重连、状态上报、OTA/FOTA 证据边界。
- BSP/Linux：启动、设备树、dmesg、sysfs/procfs、驱动验证。

模板见 `templates/project-bullets-template.md`。

## Hardware Debug Description Patterns

硬件调试必须具体到现象、仪器、排查路径和验证方式。不要把“会接线”写成“硬件设计”。

常见追问：

- 串口无输出：供电、GND、TX/RX、波特率、BOOT0/NRST、时钟、串口映射。
- I2C 无 ACK：地址、上拉、时序、供电、电平、逻辑分析仪波形。
- ADC 漂移：参考电压、采样周期、阻抗、滤波、接地、校准。
- 下载失败：SWD/JTAG、BOOT0、NRST、供电、芯片锁定、驱动。

模板见 `templates/hardware-debug-template.md`。

## RTOS and Platform Routing

- FreeRTOS/RT-Thread/Zephyr：只有真实任务、队列、信号量、互斥锁、事件组、定时器或栈水位证据时，才能写项目经验。
- 只看教程或跑 demo：写“了解/学习中”，并给补练习任务。
- BSP/Linux：没有 Device Tree、dmesg、sysfs/procfs、驱动验证证据时，不写驱动开发经验。
- Mbed/Mbed OS：作为退场技术处理，除非 JD 明确要求或用户有遗留项目证据，不作为主路线包装。

## Interview Follow-up Generation

面试追问必须贴合岗位族：

- STM32/MCU：为什么选该外设，时钟/中断/DMA 怎么配，异常怎么复现和验证。
- 嵌入式测试：测试用例、边界、回归、缺陷闭环、日志和报告。
- 硬件联调：供电、接地、波形、时序、复位、下载失败定位。
- 工控：Modbus 帧、CRC、轮询、超时、抗干扰、故障日志。
- IoT：联网、MQTT、心跳、断线重连、状态上报、低功耗和 OTA 边界。
- BSP/Linux：设备树、pinmux、dmesg、sysfs、U-Boot/Kernel 边界。

主题库见 `references/embedded-interview-topics.md`。

## Apply Message Patterns

只生成文本草稿和人工确认清单。不得自动投递、自动私信、批量骚扰 HR 或绕过平台规则。

投递沟通必须：

- 短句说明目标岗位族和最相关项目；
- 对短板使用诚实表达；
- 不承诺虚假年限、企业经验、客户交付或量产经历；
- 在发送前提醒用户人工确认。

模板见 `templates/application-message-template.md`。

## Role Routing Rules

当 JD 或用户经历跨多个方向，按证据强度排序：

1. 有项目代码/日志/报告/波形的岗位族优先。
2. 只有学习记录的能力降级为补充项。
3. 开发、测试、联调、BSP/Linux、IoT、工控、车载测试不得混写。
4. 若 JD 中有 CANoe/HIL/ISO 26262/ASPICE/医疗/功能安全等高门槛词，必须检查真实证据和初级边界。

## Platform Boundaries

- 可以生成岗位筛选表、投递文案、HR 跟进话术、复盘清单。
- 不得自动投递。
- 不得自动私信。
- 不得绕过平台规则。
- 不可以自动提交申请、自动私信、绕过反爬或平台限制、冒充用户发送消息。
- 不协助伪造学历、证书、薪资、客户、团队规模、项目上线、量产或企业背书。

## Pressure Scenarios

执行前或修改后，用 `tests/pressure-scenarios.md` 检查是否能拦住：

- GPIO 冒充 RTOS；
- 课程项目冒充量产；
- UART 冒充 Modbus 协议栈；
- 无 CANoe/HIL/OTA/BSP 证据却包装成项目经验；
- 自动投递或自动私信；
- “包装成两年经验”等明确造假。

## Common Mistakes

| 错误 | 正确处理 |
|---|---|
| 把普通求职模板换成嵌入式关键词 | 先岗位族路由，再选证据和模板 |
| 把“了解”写成“熟悉” | 标 `needs_proof` 并降级表达 |
| 把测试岗写成开发岗 | 改用测试用例、日志、缺陷闭环证据 |
| 把课程项目写成企业项目 | 保留项目性质，强调个人职责 |
| 把会接线写成硬件设计 | 写硬件联调/调试支持边界 |
| 自动投递或自动私信 | 只给草稿，用户人工确认 |

## Output Formats

默认中文输出。根据任务选择：

- 候选人画像：目标、岗位族、证据、风险、补证据任务。
- JD 深拆：岗位族、要求、匹配、短板、追问、投递建议。
- 简历 bullet：可写版本、证据来源、可追问点、风险等级。
- 面试追问：按岗位族分组，每题附证据需求和回答边界。
- 投递文案：场景、草稿、人工确认提醒、禁止自动发送。

## Reference Files

- `references/embedded-role-keywords.md`：岗位族关键词和证据要求。
- `references/embedded-technical-map.md`：嵌入式技术地图。
- `references/embedded-market-notes.md`：2026-06-29 市场备注与设计影响。
- `references/embedded-interview-topics.md`：面试主题库。
- `references/evidence-status-guide.md`：证据状态和降级表达。

## Acceptance Checklist

修改本 Skill 后，必须检查：

- `SKILL.md` frontmatter 合法，description 只写触发条件。
- `references/` 承载重知识，`SKILL.md` 不堆技术百科。
- `templates/` 可直接复用，`examples/` 是嵌入式真实场景。
- `tests/pressure-scenarios.md` 覆盖反夸大和平台边界。
- `NOTICE.md` 说明 `career-ops` TRADEMARK 边界和非官方身份。
- 项目没有写成 `career-ops` 或 `JobOK` 官方版本。
- 不是泛求职 Skill 只替换少量嵌入式关键词。

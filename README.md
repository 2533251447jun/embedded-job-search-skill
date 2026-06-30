# embedded-job-search-skill

`embedded-job-search-skill` 是一个独立命名的 Codex/Agent Skill 项目，用于帮助候选人基于真实经历准备国内嵌入式相关岗位求职。

它服务的不是泛求职场景，而是 STM32/MCU 固件、嵌入式测试、硬件调试/联调、IoT、工业控制、BSP/驱动/Linux、车载通信测试、医疗/仪器/安防/消费电子等岗位族。

## 来源与许可证

本项目受到以下 MIT 项目的启发，并在独立命名、重写内容、重构领域逻辑的前提下进行二次开发：

- `career-ops`: https://github.com/santifer/career-ops
- `JobOK`: https://github.com/GresonKwan/JobOK

`career-ops` 的代码可按 MIT License 复用，但其名称、品牌、logo、视觉资产、官方背书、认证、商业命名等不属于 MIT 代码许可的一部分。本项目不是 `career-ops` 或 `JobOK` 的官方版本，也不代表原作者认可、赞助、认证或维护。

JobOK 审计结论：未发现额外 NOTICE/TRADEMARK 文件。

## 本项目新增的嵌入式定向能力

- 岗位族路由：先判断 STM32/MCU、测试、硬件联调、IoT、工控、BSP/Linux、车载测试等方向。
- 证据链：所有简历内容落到 `fact`、`inference`、`user_preference`、`needs_proof` 或证据状态。
- 项目边界：课程、实训、个人、实习、企业项目分别表达，不混成量产或客户项目。
- 嵌入式技术地图：外设、RTOS、协议、硬件调试、测试、Linux/BSP、功能安全边界。
- 反夸大测试：用压力场景阻止把“了解”写成“熟悉”、把 demo 写成项目主导。

## 支持的岗位族

- STM32 / MCU 固件
- 嵌入式测试
- 硬件调试 / 硬件联调
- IoT 设备端
- 工业控制 / 数据采集
- BSP / 驱动 / 嵌入式 Linux 初级方向
- 车载嵌入式 / 通信测试
- 医疗 / 仪器仪表 / 安防 / 门禁 / 消费电子

## 支持的技术方向

C/C++、STM32、GD32、ESP32、51、ARM Cortex-M、Keil/MDK、STM32CubeMX、GCC、J-Link、ST-Link、GPIO、UART、I2C、SPI、ADC、DMA、Flash、RTC、Watchdog、FreeRTOS、RT-Thread、Zephyr、RS485、Modbus、CAN、UDS、MQTT、BLE、Wi-Fi、OTA/FOTA、示波器、逻辑分析仪、万用表、测试用例、缺陷复现、BSP、Device Tree、U-Boot、Linux Kernel。

## 适用人群

- 应届或初级嵌入式求职者。
- 从电子、自动化、物联网、通信、计算机等方向转嵌入式的候选人。
- 有课程、实训、个人项目或少量实习经验，需要整理项目证据的人。
- 想把嵌入式测试、硬件联调、工控、IoT、BSP/Linux 方向区分表达的人。

## 不适用场景

- 纯互联网、运营、销售、设计等非嵌入式求职任务。
- 伪造学历、实习、工作年限、项目、量产、客户、商业成果、证书或薪资结果。
- 自动投递、自动私信、绕过平台规则、批量骚扰 HR。
- 需要法律、财务、医疗、移民等专业意见的任务。

## 安装方式

将本目录作为 Skill 项目保存在本地。若要安装到某个 Agent 环境，请按该环境的 Skill 安装规则复制或引用目录。

公开仓库中不记录个人本地路径。安装时请将项目目录复制或克隆到你的 Agent 支持的 Skill 目录，并按对应环境的安装规则启用。

## 使用方式

向 Agent 提出嵌入式求职任务，例如：

- “帮我分析这个 STM32/Modbus 岗位 JD。”
- “把我的 STM32 + I2C + OLED 课程项目改写成简历 bullet。”
- “我只做过串口收发，能不能投嵌入式测试岗？”
- “帮我准备硬件联调岗面试追问。”
- “写一段 Boss 直聘开场白，发送前我会人工确认。”

## 目录结构

```text
embedded-job-search-skill/
  SKILL.md
  README.md
  LICENSE
  NOTICE.md
  CHANGELOG.md
  examples/
  templates/
  references/
  tests/
```

## 平台边界与人工确认

本项目只生成分析、草稿、清单和建议。所有投递、私信、资料修改、平台操作都必须由用户人工确认并手动执行。

不得使用本项目绕过招聘平台规则、批量骚扰、自动提交申请、自动私信 HR，或伪装成人类操作。

## 免责声明

本项目只帮助优化真实经历表达、岗位匹配、项目整理、面试准备和投递复盘，不帮助伪造学历、工作经历、项目经历、量产经验、客户案例、商业成果、证书、薪资结果、团队规模、上线范围或企业背书。

AI 生成内容可能存在错误。用户必须在发送简历、投递文案或面试材料前人工核对。

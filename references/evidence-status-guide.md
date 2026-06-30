# Evidence Status Guide

Use these labels before turning any embedded experience into resume text, interview prep, or application messages.

| Status | Meaning | Resume handling |
|---|---|---|
| `verified` | Evidence is directly reviewable: code, report, waveform, logs, screenshots, repository, demo video, or uploaded files. | Can write as experience if wording matches evidence. |
| `partially_verified` | Some evidence exists, but scope, ownership, or outcome is incomplete. | Write conservatively and list missing proof. |
| `user_claimed` | User says it happened, but no artifact is available. | Ask follow-up questions; avoid strong claims. |
| `needs_proof` | User says “should know”, “watched videos”, “want to write”, or evidence is too weak. | Do not put into resume as experience. |
| `not_allowed` | Fabrication, false degree, fake internship, fake client, fake production, auto-apply, auto-DM, or platform bypass. | Refuse and offer truthful alternative. |

## Examples

- 用户上传 STM32 代码、串口日志和演示视频：`verified` or `partially_verified`, depending on whether ownership and behavior are clear.
- 用户口述“做过 I2C OLED”：`user_claimed` until code, wiring photo, display photo, or debug notes are supplied.
- 用户说“应该会 FreeRTOS”：`needs_proof`; ask for task, queue, semaphore, timer, and stack-watermark evidence.
- 用户要求“写成两年经验”：`not_allowed`; refuse the false claim and write an entry-level positioning version.

## Downgrade Language

| Unsupported phrase | Safer phrase |
|---|---|
| 熟练 FreeRTOS | 学习过 FreeRTOS 基础概念，正在补充任务通信实践 |
| 主导 Modbus 协议栈 | 完成 UART 基础收发，正在学习 Modbus RTU 帧解析 |
| 硬件设计经验 | 配合硬件联调，完成供电/接线/串口日志排查 |
| 量产项目 | 课程/个人项目，完成本地功能验证 |
| 客户交付 | 项目演示或内部验证，未涉及客户交付 |
| 精通寄存器 | 使用 CubeMX/HAL 完成配置，正在学习寄存器级实现 |

## Required Questions Before Strong Claims

- Who owned the code or test report?
- What artifact can be shown?
- What was the candidate's personal responsibility?
- Was it course, personal, internship, or enterprise work?
- How was the result verified?
- What would an interviewer likely ask, and can the candidate answer with evidence?

# Embedded Profile Example

## 基本目标

- 目标：应届/初级嵌入式软件或嵌入式测试岗位。
- 目标城市：深圳、东莞、广州。
- 目标岗位族：STM32/MCU 固件、嵌入式测试、硬件联调助理。
- 不优先：BSP/Linux 驱动、车载 HIL、功能安全岗位。

## 当前技术栈

- `fact`: 做过 STM32F103 课程项目，使用 CubeMX/HAL 配置 GPIO、I2C、ADC、UART。
- `fact`: 用 OLED 显示 ADC 采样值，用串口输出调试日志。
- `fact`: 用万用表检查过供电和电平。
- `user_preference`: 更想找深圳/东莞的初级固件或测试岗位。
- `inference`: 适合先投 STM32/MCU、硬件联调助理、嵌入式测试初级岗位。
- `needs_proof`: FreeRTOS、Modbus、示波器、低功耗、BSP/Linux 尚无项目证据。

## 真实项目证据

| 证据 | 状态 |
|---|---|
| CubeMX 配置截图 | `partially_verified` |
| Keil 工程代码 | `verified` if uploaded |
| 串口日志 | `partially_verified` |
| OLED 显示照片 | `partially_verified` |

## 缺失证据

- 示波器波形截图。
- 完整测试报告。
- FreeRTOS 任务 demo。
- RS485/Modbus 帧解析记录。

## 风险项

- 不能写“熟悉 FreeRTOS”。
- 不能写“熟练硬件调试”。
- 不能把课程项目写成企业项目或量产项目。

## 推荐岗位族

- STM32/MCU 初级固件：可投，需补外设调试细节。
- 嵌入式测试：可投，需补测试用例和缺陷复现记录。
- 硬件联调助理：谨慎投，需诚实说明仪器经验边界。

## 不推荐岗位族

- BSP/Linux 驱动：缺少设备树、dmesg、驱动验证证据。
- 车载 HIL/UDS：缺少 CANoe/CANalyzer、HIL、UDS 实操证据。
- 功能安全/医疗认证：缺少规范和项目证明。

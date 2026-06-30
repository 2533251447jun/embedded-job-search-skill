# Embedded Technical Map

Use this map to route JD requirements, candidate evidence, interview questions, and resume bullets. Do not copy the full map into final answers; load only the relevant section.

## C Language and Firmware Basics

- C 语言基础 / C basics: pointer 指针, array 数组, string 字符串, struct 结构体, enum 枚举, union 联合体, function pointer 函数指针, macro 宏, conditional compilation 条件编译, header files 头文件, `.c/.h` separation 分层。
- Embedded C / 嵌入式 C: `volatile`, `const`, `static`, `extern`, bit operation 位操作, register bit 寄存器位, memory alignment 内存对齐, stack 栈, heap 堆, map file 映射文件。
- Firmware patterns / 固件模式: state machine 状态机, callback 回调, ring buffer 环形缓冲区, timeout 超时机制, error code 错误码, defensive programming 防御式编程。
- Debug basics / 调试基础: HardFault, call stack 调用栈, register 寄存器, memory 内存, log analysis 日志分析, minimal reproduction 最小复现。

## MCU Platforms and Toolchains

- MCU families: STM32F1/F4/G0/G4/H7/L, GD32, ESP32, 51, NXP, Nordic, TI, Renesas, Infineon, RISC-V MCU.
- Cores: ARM Cortex-M0/M3/M4/M7/M33, Cortex-A, RISC-V.
- Tools / 开发工具: Keil / MDK, IAR, STM32CubeIDE, STM32CubeMX, VS Code, Eclipse, GCC, Clang, Make, CMake.
- Debug/download / 调试下载: ST-Link, J-Link, CMSIS-DAP, SWD, JTAG, OpenOCD, GDB, serial download 串口下载, BOOT0, NRST, download-failure diagnosis 下载失败定位。

## MCU Peripherals

- GPIO, EXTI 外部中断, NVIC 中断控制, RCC 时钟, SysTick, TIM 定时器, PWM, input capture 输入捕获, output compare 输出比较, encoder 编码器。
- UART/USART 串口, I2C, SPI, QSPI, ADC, DAC, DMA / Direct Memory Access 直接存储器访问。
- Flash, EEPROM 模拟, RTC, watchdog 看门狗 / IWDG/WWDG, Clock Tree 时钟树, PLL, low power mode 低功耗, PVD, CRC。
- CAN, USB CDC, SDIO/FatFS: only write as experience when there is real proof.

## RTOS and Real-Time Systems

- FreeRTOS, RT-Thread, Zephyr, CMSIS-RTOS, CMSIS RTX, ThreadX.
- Task division, priority, time slice, queue, semaphore, mutex, event group, software timer, task notification.
- Interrupt/task communication, critical section, stack overflow, deadlock, priority inversion, real-time response, task period, Tick, Idle Hook, Tickless low power.
- Evidence needed: runnable demo or project code, task diagram, logs, stack-watermark notes, bug diagnosis.

## Communication and Industry Protocols

- UART, RS232, RS485, Modbus RTU, Modbus TCP.
- CAN, CANopen, J1939, UDS.
- TCP/IP, UDP, HTTP, HTTPS 了解, MQTT, CoAP, WebSocket 了解, OPC UA 了解, EtherCAT 概念, Profinet 概念.
- BLE, Wi-Fi, NB-IoT, 4G Cat.1, LoRa and Zigbee when JD mentions them.
- OTA/FOTA, disconnect reconnect, heartbeat, protocol frame, CRC, frame header/tail, timeout retry, device status report, acquisition cycle, multi-device polling.
- 初级边界：无真实协议帧、日志、代码或测试记录时，只写“了解 / 学习中 / 概念接触”，不写项目经验。

## Hardware Debug and Instruments

- Tools / 工具: 万用表 / multimeter, 示波器 / oscilloscope, 逻辑分析仪 / logic analyzer, 串口助手 / serial terminal, USB-TTL, CAN 分析仪 / CAN analyzer, 总线分析仪 / bus analyzer, 可调电源 / bench power supply, current meter 电流表.
- Hands-on basics: soldering, jumper wires, schematic reading, PCB identification, power check, ground check, level check, pull-up/pull-down, reset circuit, crystal.
- Fault topics: I2C ACK, SPI CPOL/CPHA, UART baud rate, no serial output, ADC drift, interrupt not firing, download failure, reset abnormal, ESD/EMC basics, anti-interference.
- Evidence: waveform screenshot, protocol frame log, test record, reproduction steps.

## Embedded Testing

- Test planning, test case, functional test, interface test, integration test, system test, boundary test, stress test, long-run test, aging test, exception injection, regression test.
- Black-box, white-box, unit test, Unity, Ceedling, HIL, SIL, CANoe, CANalyzer.
- Serial automation, Python test scripts, log analysis, defect reproduction, defect closure, test report, version record, requirements traceability.
- Test coverage should only be written when there is real measurement or report evidence.

## BSP/Linux/Driver

- ARM boot flow, startup file, linker script, pinmux, HAL/LL/register relationship, interrupt vector table.
- Bootloader, U-Boot, Linux Kernel, Device Tree, Kconfig, Makefile, CMake, GCC, cross compilation.
- UART console, SPI/I2C/GPIO Linux driver basics, dmesg, sysfs, procfs, board bring-up, schematic-to-device-tree mapping.
- 初级边界：修改 Device Tree、编译 demo、跑通教程只能写“了解/实验”，不得写 BSP 负责人、驱动专家或板级 bring-up 负责人。

## Engineering Quality and Safety

- Git, README, version management, driver/application layering, configuration files, log system, error codes, watchdog recovery, power-loss protection, exception record.
- Static analysis, MISRA C, ISO 26262, IEC 61508, ASPICE, DO-178C, SBOM, firmware security, Secure Boot, encrypted upgrade, rollback, firmware CI/CD.
- These are high-risk resume claims. Use “了解/学习中” unless the user has real artifacts.

## Junior Candidate Writable Range

- Basic peripherals with code and demo evidence.
- Clear test cases and logs.
- Hardware debug participation with real fault records.
- Protocol learning with simple frame parsing.
- RTOS concept or demo when truthfully labeled.
- BSP/Linux concepts when not written as driver ownership.

## High-Risk Not Writable Without Proof

- “精通/主导/架构设计”.
- Mass production, customer delivery, commercial results.
- CANoe/HIL/SIL, ISO 26262/ASPICE, medical certification, industrial safety.
- OTA/FOTA deployment, Secure Boot, encrypted upgrade, rollback.
- Full protocol stack design when only UART bytes were sent.

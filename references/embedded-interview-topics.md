# Embedded Interview Topics

Use this file to generate role-specific follow-up questions. Each topic should expose evidence, junior boundaries, and exaggeration risk.

| Topic | Interviewer may ask | Evidence needed | Junior boundary | High-risk exaggeration |
|---|---|---|---|---|
| C language | How do `volatile`, `static`, pointer, struct, and macro affect firmware? | Code snippets, bug notes | Explain used cases, not compiler theory overload | Claiming MISRA/static-analysis ownership without proof |
| STM32 peripherals | How did you configure GPIO/UART/I2C/SPI/ADC/TIM? | CubeMX config, code, board behavior | HAL use is acceptable if stated | Calling HAL setup “register mastery” |
| Interrupts | Why use interrupt instead of polling? How handle shared data? | ISR code, flags, ring buffer | Know latency and race basics | Claiming high-performance design without measurement |
| DMA | When is DMA useful? How verify completion? | DMA config, callback/logs | If only read about it, say learning | Writing DMA optimization without code |
| UART | Baud rate, frame format, buffer overflow handling? | Serial logs, ring buffer code | Basic send/receive is entry-level | Calling it protocol stack design |
| I2C | What causes no ACK? How did you debug it? | Wiring, pull-up, logic analyzer/waveform | If no analyzer, explain learning boundary | Claiming waveform analysis without use |
| SPI | CPOL/CPHA, chip select, timing issue? | Code and captured behavior | Explain simple device communication | Claiming high-speed bus optimization |
| ADC | Sampling time, reference voltage, drift handling? | Readings, filter, calibration notes | State basic acquisition clearly | Fabricating precision/accuracy results |
| TIM/PWM | Timer clock, period, duty cycle, output verify? | Config, waveform or LED/motor behavior | Basic PWM is acceptable | Claiming motor-control expertise from LED PWM |
| Flash | How store parameters safely? | Flash write code, power-loss handling | Basic storage only if tested | Claiming robust persistence without tests |
| Watchdog | Why and how feed watchdog? | Fault/reset logs | Know purpose and reset behavior | Claiming safety design without system tests |
| FreeRTOS | Task split, priority, queue/semaphore, stack overflow? | Task code, logs, debug notes | Tutorials are “学习中” | Writing “熟悉调度” after videos only |
| RT-Thread | Components, threads, IPC, device framework? | Project or demo artifacts | State demo scope | Claiming production RTOS use |
| RS485/Modbus | Frame format, CRC, timeout, polling? | Frame logs, CRC code, device test | Simple parser is good if honest | Claiming protocol stack from UART |
| CAN | ID, frame, bus analysis, DBC? | Bus logs/tool screenshots | Learn basics if no tool | Claiming CANoe/CANalyzer without use |
| MQTT | topic, QoS, reconnect, heartbeat? | Broker logs, device logs | Basic publish/subscribe is okay | Claiming cloud architecture ownership |
| Hardware debug | How check power, ground, reset, clock, waveforms? | Instrument notes, photos, screenshots | Say “配合联调” when appropriate | Writing hardware design when only wired |
| Embedded testing | How design cases, reproduce bugs, close defects? | Test report, issue record, logs | Manual functional test is valid if labeled | Claiming system testing without report |
| BSP/Linux | Device tree, dmesg, sysfs, driver verification? | Boot logs, DTS, commands | Concepts vs hands-on must be split | Claiming driver development without board |
| IoT | reconnect, OTA, low power, device state? | Logs, power data, firmware flow | Basic module use is fine | Claiming FOTA deployment without proof |
| Industrial field issues | interference, timeout, device offline, fault record? | Long-run logs, retry logic | Entry-level can discuss observed cases | Claiming field delivery without site work |
| Project boundary | What did you personally do? Course or enterprise? | Timeline, repo, screenshots | Honest ownership earns trust | Inflating demo into product |

## Question Generation Rule

For each resume bullet, generate:

1. one implementation question;
2. one debugging question;
3. one verification question;
4. one boundary question that checks whether the candidate is exaggerating.

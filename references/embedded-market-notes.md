# Embedded Market Notes

Date: 2026-06-29

These notes convert current visible market signals into Skill design rules. They are not a broad industry report.

## Research Basis

Public job pages and searches visible during planning showed recurring embedded JD terms around STM32, C/C++, RTOS/FreeRTOS, RS485/Modbus, UART/I2C/SPI, hardware debugging, testing reports, Linux/drivers, CAN/UDS/HIL, and junior firmware roles. Mbed/Mbed OS should be treated as a retiring technology because Arm announced Mbed site/archive access and Mbed OS end-of-life for July 2026.

Useful source URLs recorded during planning:

- https://cn.indeed.com/q-%E5%B5%8C%E5%85%A5%E5%BC%8F%E8%BD%AF%E4%BB%B6%E5%BC%80%E5%8F%91%E5%B7%A5%E7%A8%8B%E5%B8%88-%E8%81%8C%E4%BD%8D.html
- https://www.zhipin.com/
- https://jobs.siemens.com/en_US/externaljobs/JobDetail/505753
- https://os.mbed.com/blog/entry/Important-Update-on-Mbed/

If a future environment cannot access the web, state that current market information cannot be freshly verified and rely on this dated note plus user-provided JD text.

## Design Implications

- Initial embedded roles still reward real project detail more than broad “熟悉嵌入式” wording.
- STM32/MCU remains a useful entry route when paired with specific peripherals, debugging notes, and verification evidence.
- RTOS is valuable, but only write project experience when the candidate can explain task division, synchronization, stack issues, or timing behavior.
- Industrial control and data acquisition roles need protocol/frame evidence: RS485 wiring, Modbus RTU/TCP, CRC, polling, timeout, fault logs.
- IoT roles need device-side boundary clarity: connection flow, MQTT topics, reconnect, heartbeat, device logs, OTA/FOTA proof.
- Embedded testing roles should be expressed through test cases, logs, waveforms, defect reproduction, reports, and regression, not firmware ownership.
- Hardware debug/joint debug roles can fit junior candidates when they can explain instruments, power/ground checks, wiring, reset, clock, and fault reproduction.
- BSP/Linux roles have a higher evidence bar: boot logs, device tree, dmesg/sysfs, driver verification, cross compilation.
- Vehicle/medical/function-safety roles require careful boundaries. Without CANoe/HIL/ASPICE/ISO 26262/medical compliance proof, write “了解/学习中”.

## Candidate Strategy

- Prefer 2-3 evidence-rich projects over many vague keywords.
- Use role-family-specific resumes instead of one generic embedded resume.
- Treat missing evidence as a task list: add logs, screenshots, README, test records, waveform captures, and reproduction steps.
- Avoid writing Mbed/Mbed OS as a main career route unless the JD requires legacy support.

## Fraud and Platform Boundary Reminders

- Reject fake internships, fake production, fake customer delivery, fake code repositories, and fake years of experience.
- Do not auto-apply, auto-DM, bypass platform rules, scrape prohibited pages, or impersonate the user.
- Provide drafts and checklists; the user sends or submits manually.

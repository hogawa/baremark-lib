# baremark-lib

An instrumentation library for bare-metal testing and benchmarking of cryptographic libraries.

## Common utilities

- Basic GPIO (LED blink)
- UART with retargeted `printf()`
- Cycle counter
- PRNG (if available)

## Target platforms

|       CPU      |           Board          |  Firmware   | PRNG support  | Label           |
|:--------------:|:------------------------:|:-----------:|:-------------:|:---------------:|
| ARM Cortex-M0+ | Raspberry Pi Pico        | pico-sdk    |               |                 |
| ARM Cortex-M0  | Infineon XMC X2Go        |             |               |                 |
| ARM Cortex-M3  | STM32F103-Bluepill       | libopencm3  | NO            |                 |
| ARM Cortex-M3  | SmartFusion2 Maker Board | SoftConsole | YES           |                 |
| ARM Cortex-M3  | NUCLEO-F207ZG            | CubeMX      | YES           | `NUCLEO_F207ZG` |
| ARM Cortex-M4  | STM32F4-Discovery        | libopencm3  | YES           |                 |
| ARM Cortex-M33 | NUCLEO-H563ZI            | CubeMX      | YES           |                 |
| ARM Cortex-M33 | NUCLEO-WBA52CG           | CubeMX      | YES           |                 |
| ARM Cortex-A9  | Avnet MiniZed            | Xilinx BSP  | YES           |                 |
| ARM Cortex-A9  | Avnet MicroZed           | Xilinx BSP  | YES           |                 |
| ARM Cortex-A53 | Raspberry Pi 3B+         | N.A.        | YES           |                 |

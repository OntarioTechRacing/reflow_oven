# Reflow Oven

---

# Prerelease Version

Reflow oven meant to be used by hardware and electronics. Includes various fixes

- Lack of source code. This repo provides the source code in addition to the binaries.
- Translation of German Code comments. I have kept the original text, and appended the translation side by side. Please do not delete the german comments.
- fix of several while loop and iterative mistakes. Modularization

## BOM

Note that this may be subject to change depending on department requirements

| Part                | Component                              | Quantity |
| ------------------- | -------------------------------------- | -------- |
| Microcontroller     | Blue Pill                              | 1        |
| Nextion Display     | TBD                                    | 1        |
| USB Power Source    | TBD                                    | 1        |
| Toaster Oven        | Generic                                | 1        |
| Thermo-coupler      | Any Generic (Ideally Type L or type J) | 1        |
| Logic Level Shifter | 3.3V to 5V (any generic)               | 1        |

# Block Diagram

# Configuration & Wiring

![Pinout View](Documentation/Pinout%20View.png)

## Logic

| Bluepill Pin | Configuration  | Connecting Component | PIN # |
| ------------ | -------------- | -------------------- | ----- |
| PA14         | SYS_JTCK-SWCLK |                      | 38    |
| PA13         | SYS_JTMS-SWDIO |                      | 34    |
| PA10         | USART1_RX      |                      | 31    |
| PA9          | USART1_TX      |                      | 30    |
| PA8          | TIM_CH1        |                      | 29    |
| PA6          | SD             |                      | 16    |
| PA5          | CK             |                      | 15    |
| PA4          | CS             |                      | 14    |
| PD1-OSC_OUT  | RCC_OSC_OUT    |                      | 6     |
| PD0-OSC_IN   | RCC_OSC_IN     |                      | 5     |

## Power

| Function | Pin #'s    |
| -------- | ---------- |
| VDD      | 48, 36, 24 |
| VSS      | 47, 35, 23 |
| VDDA     | 9          |
| VSSA     | 8          |
| VBAT     | 1          |

## Reserved

| Name  | #   | Function    |
| ----- | --- | ----------- |
| NRST  | 7   | reset_state |
| BOOT0 | 44  | reset_state |

# Legend for GUI

![b0](Documentation/b0.png)
![b4](Documentation/b0.png)
![b6](Documentation/b0.png)

| Prefix             | Description         |
| ------------------ | ------------------- |
| 'b'  is for button | Meant to be pressed |
| 't' is for text    | Meant to be read    |

# Future-Proofing:

- Add support for multiple thermocouplers

- Add buzzer for cooldown period

# To Do:

update stm binary and update nextion binary

refactor code for easier use

Pcb revision 1

# Reflow Oven

---

# Beta Version

Reflow oven meant to be used by hardware and electronics. Includes various fixes

- Lack of source code. This repo provides the source code in addition to the binaries.
- Translation of German Code comments. I have kept the original text, and appended the translation side by side. Please do not delete the german comments.
- fix of several while loop and iterative mistakes. (lines 563, 620)

## BOM

Note that this may be subject to change depending on department requirements

| Part                | Component       | Quantity |
| ------------------- | --------------- | -------- |
| Microcontroller     | Blue Pill       | 1        |
| Nextion Display     | Small One       | 1        |
| USB Power Source    | TBD             | 1        |
| Toaster Oven        | The one we have | 1        |
| Thermo-coupler      | The one we have | 1        |
| Logic Level Shifter | a 5V one        | 1        |

# Block Diagram

# Configuration & Wiring

# Legend for GUI

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

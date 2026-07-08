# STM32F103 Minimal Development Board (v1.1)
![Board 3D Render](https://github.com/halilozgg-blip/STM32F103-Minimal-Development-Board-v1.1-/blob/main/STM32F103%20IMAGES%20AND%20DOCs/STM32_Minimal_DevBoard_v1.1(3).png)
![KiCad](https://img.shields.io/badge/Designed_in-KiCad_9.0-blue.svg)
![Hardware](https://img.shields.io/badge/Hardware-Open_Source-orange.svg)

##  Project Overview
This project is a custom-designed **STM32F103C8T6** development board created using **KiCad 9.0**. It provides a compact and reliable hardware platform for embedded software development, rapid prototyping, and educational projects.

The design focuses on clean power distribution, hardware protection, modular architecture, and debugging convenience while following recommended PCB design practices.

##  Design Goals
* **Reliable Hardware:** Design a stable and reusable STM32 development platform.
* **Easy Development:** Provide essential interfaces required for firmware development and debugging.
* **Good PCB Practices:** Follow clean schematic organization and PCB layout guidelines.
* **Open Source:** Make the project easy to understand, reproduce, and modify.

##  Key Features

###  Power & Protection
* **USB Type-C** Power Input.
* **USBLC6-2SC6** TVS diode for ESD protection on USB data lines.
* **500 mA** Resettable PTC Polyfuse for overcurrent protection.
* **AMS1117-3.3V** linear regulator providing a stable 3.3V supply.
* Decoupling capacitors placed according to STM32 hardware design recommendations.

###  Microcontroller Hardware
* **STM32F103C8T6** ARM Cortex-M3 microcontroller.
* External crystal oscillator.
* Hardware reset circuit.
* Pull-down resistor on `BOOT0` for reliable boot configuration.
* **SWD** programming and debugging interface.
* Clearly labeled test points for debugging and measurements.

###  Development Features
* User LED.
* User push button.
* GPIO expansion headers.
* Modular schematic hierarchy for easier maintenance and future expansion.

## 📂 Repository Structure
  ```text
STM32F103_Minimal_Development_Board_v1.1
│
├── HARDWARE/        # KiCad Project, Schematics, and PCB Layout
├── PRODUCTION/     # Gerber Files, Drill Files, and Manufacturing Outputs
└── STM32F103 IMAGES AND DOCS/
    ├── Schematic PDF, PCB Images
    ├── 3D Renders
    └── Project Documentation
  ```
#  Hardware Summary

| Component | Description |
| :--- | :--- |
| **MCU** | STM32F103C8T6 |
| **Core** | ARM Cortex-M3 |
| **Operating Voltage** | 3.3 V |
| **Power Input** | USB Type-C |
| **Debug Interface** | SWD |
| **PCB Design** | KiCad 9.0 |

##  Future Improvements
* USB communication support.
* Additional protection circuitry.
* Boot mode selection jumper.
* CAN interface.
* External SPI Flash & I²C EEPROM.
* Additional status indicators.

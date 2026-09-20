<h1 align="center">Md. Shohanur Rahman</h1>

<p align="center">
  <b>Embedded Systems Engineer</b><br/>
  Firmware &nbsp;·&nbsp; PCB Hardware &nbsp;·&nbsp; Motor Control &nbsp;·&nbsp; Power Electronics
</p>

<p align="center">
  <i>I build embedded systems across hardware and firmware — from schematic and PCB to bring-up, debugging and production.</i>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/engr-shohanur-rahman-181a69250">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:shohanur.dev@gmail.com">
    <img src="https://img.shields.io/badge/Email-shohanur.dev%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</p>

---

## About

I'm an **Embedded Systems Engineer** working in Research & Innovation, with hands-on experience across embedded firmware, PCB hardware, power electronics and product development.

My work spans the complete engineering cycle:

**Requirement → Schematic → PCB → Firmware → Bring-up → Validation → Production**

I work primarily with **Embedded C, STM32, PIC, AVR/Atmel, ESP32 and Altium Designer**, with a strong interest in bare-metal firmware, reusable software architecture, motor control and real-time embedded systems.

Some of my professional work is proprietary, so this profile focuses mainly on my personal projects, open-source work and engineering experiments.

---

## Core Expertise

### Embedded Firmware

* Embedded C and bare-metal programming
* STM32 / ARM Cortex-M
* PIC and AVR / Atmel
* ESP32
* GPIO, ADC, PWM and timers
* Interrupts and DMA
* UART, SPI and I²C
* Peripheral driver development
* HAL / BSP / layered firmware architecture
* Real-time embedded systems
* Firmware debugging and hardware bring-up

### Hardware & PCB Design

* Schematic design
* Multi-layer PCB design
* Altium Designer
* MCU-based control boards
* Power electronics PCBs
* Gate-driver circuits
* Current sensing
* Power supply design
* Hardware bring-up and debugging
* Design for manufacturability

### Motor Control & Power Electronics

* BLDC motor control
* Six-step commutation
* Sensorless motor control
* FOC development
* Sliding Mode Observer (SMO)
* Current measurement
* Gate drivers
* Inverter / power-stage design
* Buck converters
* PWM-based power control

---

## Professional Experience

### Walton Hi-Tech Industries PLC

**Research & Innovation — Refrigerator** · 2024 – Present

Working across embedded electronics, firmware, PCB development, validation and production support for refrigerator platforms.

Selected areas of work:

* Development and evaluation of MCU-based control and display electronics
* Embedded firmware development and peripheral integration
* Multi-layer PCB design and hardware evaluation
* Hardware bring-up, debugging and validation
* Inverter-board evaluation and motor-control related development
* Root-cause analysis of hardware and field issues
* Development of lab test equipment and data-logging solutions
* Display, touch-interface and control-board development
* BOM and SOP preparation
* SMT and production-line technical support
* Component and PCB validation for product platforms

---

## Selected Personal Projects

### G4_Core_Lib

A lightweight, reusable **STM32G4 firmware framework** developed from scratch using CMSIS, CMake and ARM GNU Toolchain — without depending on CubeMX-generated application code.

```text
Application
     │
     ▼
Driver / API
     │
     ▼
HAL
     │
     ▼
BSP / Board
     │
     ▼
STM32 Hardware
```

Current development includes:

* GPIO abstraction
* TimeCore
* Logging framework
* UART driver architecture
* System clock management
* Board-level configuration
* Reusable driver interfaces

**Repository:**
https://github.com/shohanur00/G4_Core_Lib

---

### TimeCore

A reusable STM32 time-management module providing a simple application-level timing interface.

**Focus:**

* 1 ms software time base
* Hardware timer abstraction
* Interrupt-driven timekeeping
* Timer state management
* Hardware-independent application API

---

### Logger Framework

A modular embedded logging architecture designed to keep application code independent from the actual output backend.

```text
Application
     │
     ▼
Logging Frontend
     │
     ▼
Logging Core
     │
     ▼
Backend
 ┌───┼────────┐
 ▼   ▼        ▼
UART Flash    RAM
```

The architecture focuses on:

* Log levels
* Module identification
* Timestamps
* Formatted output
* UART terminal colors
* Multiple backends
* Compile-time configuration
* Testability

---

### TurboSpin V2.0

A custom **sensorless BLDC ESC** platform focused on high-speed drone motor applications.

Hardware and firmware development includes:

* STM32G431CBT6
* DRV8301 gate driver
* Three-phase inverter
* Current sensing
* External comparator
* DShot interface
* Telemetry
* Six-step commutation
* Sensorless control research
* FOC development
* Sliding Mode Observer investigation

The project combines **power electronics, embedded firmware and motor-control algorithms** in one system.

---

### Ababil FC

A custom flight-controller platform under development for long-range fixed-wing applications.

Planned hardware includes:

* STM32F405RGT6
* BMI270 IMU
* INA226 power monitor
* MS5611 barometer
* W25Q128 flash
* AT7456E OSD
* GPS
* ELRS
* microSD

Current development is focused on the hardware architecture and power subsystem.

---

## Engineering Approach

### Understand the hardware

I prefer understanding what happens below the abstraction layer — registers, peripherals, timing, signals and power paths — rather than treating hardware as a black box.

### Keep firmware modular

My preferred architecture separates:

```text
Application
    ↓
Driver / API
    ↓
HAL
    ↓
BSP
    ↓
Hardware
```

The goal is reusable code that is easier to test, maintain and port.

### Validate with measurements

I rely on measurements rather than assumptions.

Typical tools include:

* Oscilloscope
* Logic analyzer
* Signal analyzer
* Power analyzer
* Programmable AC/DC source
* ST-LINK / debugger

### Design for the real world

A working prototype is only the beginning.

I also consider:

* Component availability
* BOM discipline
* PCB manufacturability
* Production testing
* Hardware reliability
* Debugging and serviceability

---

## Toolbox

| Category            | Tools / Technologies                                           |
| ------------------- | -------------------------------------------------------------- |
| **Languages**       | C, Python                                                      |
| **MCUs**            | STM32, PIC, AVR / Atmel, ESP32                                 |
| **Firmware**        | CMSIS, Bare-metal C, HAL, BSP, Peripheral Drivers              |
| **PCB**             | Altium Designer                                                |
| **Build**           | CMake, Ninja, ARM GNU Toolchain                                |
| **Development**     | VS Code, STM32CubeIDE, Keil, MPLAB X, Atmel Studio, PlatformIO |
| **Debugging**       | Cortex-Debug, ST-LINK, SVD / Register View                     |
| **Version Control** | Git, GitHub                                                    |
| **Lab**             | Oscilloscope, Logic Analyzer, Signal Analyzer, Power Analyzer  |

---

## Current Focus

🔧 **G4_Core_Lib**
Building a reusable STM32G4 firmware ecosystem with custom HAL, drivers, timing and logging.

⚡ **TurboSpin V2.0**
Developing a sensorless BLDC ESC and exploring FOC + SMO-based position estimation.

🚁 **Ababil FC**
Designing a custom STM32-based flight-controller hardware platform.

🧪 **Embedded Testing**
Exploring ways to test firmware modules outside the target hardware using PC-based simulation and test frameworks.

📚 **Embedded Architecture**
Continuously improving reusable C architecture, driver design and hardware/software boundaries.

---

## Education

**B.Sc. in Electrical & Electronic Engineering**
Rajshahi University of Engineering & Technology (RUET) · 2023

**Thesis:**
Synchronous Buck and Boost Converter with PID Controller

---

## GitHub Projects

Some of the things I'm building here:

```text
Embedded C
├── STM32
├── PIC
├── AVR
├── ESP32
│
├── Drivers
├── HAL
├── BSP
├── Logging
├── Timing
│
├── PCB Design
├── Power Electronics
├── BLDC
├── FOC
│
└── Flight Controller
```

---

## Connect

I'm interested in connecting with engineers working in:

**Embedded Systems · Firmware · PCB Design · Motor Control · Power Electronics · Robotics · Drones · Electronics R&D**

<p align="center">
  <a href="https://www.linkedin.com/in/engr-shohanur-rahman-181a69250">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:shohanur.dev@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</p>

---

<p align="center">
  <i>Hardware gives the system a body. Firmware gives it a brain.</i>
</p>

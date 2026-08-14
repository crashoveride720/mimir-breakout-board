# Mimir ESP32-S3 Carrier Board

A compact, field-serviceable ESP32-S3 carrier board designed specifically for the Servitor Mk I (Mimir) project.

---

## Overview

The Mimir ESP32-S3 Carrier Board is an open hardware PCB that combines an ESP32-S3 development board, CAN bus transceiver, microSD interface, and field wiring terminals into a single compact assembly.

The board was created to solve a packaging problem encountered during development of the Servitor Mk I project. Using commercially available breakout boards required excessive space inside the AIU enclosure while introducing unnecessary wiring complexity.

Rather than connecting several independent modules with jumper wires, this carrier board integrates them into a single, serviceable platform.

The resulting design reduces the overall hardware footprint by approximately **one-third** while improving reliability, maintainability, and ease of assembly.

---

# Design Goals

The primary objectives of this project were:

- Reduce enclosure space requirements
- Eliminate multiple breakout boards
- Provide direct GPIO access through screw terminals
- Eliminate soldering to the ESP32 development board for field wiring
- Integrate a CAN Bus transceiver
- Integrate a removable microSD module
- Maintain access to both USB-C ports
- Allow the microSD card to be removed without disassembly
- Use inexpensive, commercially available modules
- Create a standardized hardware platform for future Servitor subsystems

---

# Features

- Compact ESP32-S3 carrier board
- Approximately **33% smaller** than using separate breakout boards
- Direct CAN Bus module support
- Direct MicroSD module support
- Screw terminal access to ESP32 GPIO pins
- Dedicated power input terminals
- No soldering required for field wiring
- USB-C ports remain fully accessible
- Push-push MicroSD card remains accessible after assembly
- Designed in KiCad
- Open Hardware

<img width="2252" height="4000" alt="20260811_180057" src="https://github.com/user-attachments/assets/52e8293f-8677-48ed-9746-66d1e9d4faf4" />
<img width="2252" height="4000" alt="20260811_180046" src="https://github.com/user-attachments/assets/a06ecb04-8c73-41f8-9754-b8e13735fd19" />
<img width="2252" height="4000" alt="20260811_175915" src="https://github.com/user-attachments/assets/117e922b-e66a-4bca-b7bc-af4d9ea6a645" />
<img width="2252" height="4000" alt="20260811_175910" src="https://github.com/user-attachments/assets/93cad456-27d9-46ff-b365-b8fe6bc3c78e" />


---

# Supported Hardware

This PCB was designed around the following commercially available modules.

While compatible alternatives may function correctly, these are the exact modules used during PCB design, fitment verification, and testing.

---

## ESP32 Development Board

**UIICPAL ESP32-S3 N16R8 Development Board**

Features

- ESP32-S3
- 16 MB Flash
- 8 MB PSRAM
- Dual USB-C
- Native USB

Amazon

https://www.amazon.com/dp/B0H2918LZD

---

## CAN Bus Transceiver

**SN65HVD230 CAN Bus Module**

This is the exact CAN module used during development.

Features

- SN65HVD230
- 3.3V operation
- ESP32 compatible
- Standard 4-pin interface

Amazon

https://www.amazon.com/dp/B0GVD5LM42

---

## MicroSD Module

**SPI MicroSD Adapter Module**

This is the exact module the PCB footprint and mechanical clearances were designed around.

Features

- SPI Interface
- Push-push (spring eject) MicroSD socket
- 3.3V operation
- Direct card access after assembly

Amazon

https://www.amazon.com/dp/B0BV8ZQ81F

---

# Component Compatibility

This PCB was mechanically designed around the modules listed above.

Other modules may function electrically, but differences in PCB dimensions, connector locations, or pin layouts may prevent proper mechanical fit.

For guaranteed compatibility, use the reference modules listed above.

---

# Repository Layout

```
docs/
    Engineering documentation
    Assembly instructions
    Wiring guides
    Bill of Materials

hardware/
    KiCad project files
    Gerbers
    STEP models
    Manufacturing outputs

images/
    Board renders
    Assembly photographs
    Reference images
```

---

# Design Philosophy

This project follows several guiding principles.

- Modular construction
- Repairable hardware
- Off-the-shelf components
- Serviceability first
- Clear documentation
- Version-controlled hardware
- Open engineering process

Every hardware revision documents both the design itself and the engineering decisions that led to it.

---

# Revision History

## Rev 1.0

- Initial hardware release
- Mechanical fit verified
- Successfully assembled using production PCBs

## Rev 1.2

- Improved silkscreen labeling
- Documentation references added
- Artwork improvements
- Increased terminal block drill diameter from **0.8 mm** to **1.0 mm** to support a wider range of commercially available terminal blocks without affecting board dimensions.

---

# Documentation

Additional documentation will be added as the project matures.

Planned documentation includes:

- Assembly Guide
- Bill of Materials (BOM)
- Pinout Reference
- Wiring Guide
- Mechanical Drawings
- Manufacturing Notes
- Engineering Notes
- Revision History

---

# License

License information will be added before the first official release.

---

## About the Servitor Project

This carrier board is one component of the larger **Servitor Mk I (Mimir)** project.

Its purpose is not simply to provide another ESP32 breakout board, but to serve as the standardized, compact, and field-serviceable hardware platform used throughout the Servitor architecture.

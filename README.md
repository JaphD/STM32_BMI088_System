# STM32_BMI088_System

This repository contains the schematic and PCB layout for a **Microcontroller-Based Hardware Design** project. The system integrates a USB-C power input, a buck converter, an STM32F0 microcontroller, and a Bosch BMI088 Inertial Measurement Unit (IMU). The design is intended for applications requiring precise motion sensing with a compact and efficient hardware setup.

## System Overview

The hardware system consists of the following key components:

- **USB-C Connector (USB4105)**:
  - Provides power input (5V nominal) and USB 2.0 full-speed connectivity to the microcontroller.
- **Buck Converter (Analog Devices LTC3405)**:
  - Steps down the 5V USB-C input to 3.3V to power the microcontroller and IMU.
- **Microcontroller (STM32F0 Series)**:
  - Core processing unit powered at 3.3V.
  - Interfaces with the USB-C connector via USB 2.0 and the IMU via SPI.
- **Inertial Measurement Unit (Bosch BMI088)**:
  - Features accelerometers and gyroscopes for motion sensing.
  - Powered at 3.3V and communicates with the microcontroller via SPI.

## Repository Contents

- `/Schematics`: Contains the schematic design files for the system.
- `/PCB_Layout`: Includes the PCB layout files, including Gerber files for fabrication.
- `/Docs`: Additional documentation, such as component datasheets and design notes.

## Getting Started

1. **Schematic Review**: Open the schematic files in your preferred EDA tool (e.g., KiCAD, Altium Designer) to review the design.
2. **PCB Fabrication**: Use the Gerber files in `/PCB_Layout` to fabricate the PCB.
3. **Assembly**: Refer to the schematic and BOM (Bill of Materials, to be added in `/Docs`) for component placement and soldering.

## Tools Used

- **EDA Software**: Altium Designer

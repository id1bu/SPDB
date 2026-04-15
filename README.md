# NEXA-POWER SPDB: Smart Power Distribution Board

[![Hardware Phase](https://img.shields.io/badge/Hardware-M1_Complete-brightgreen)](#)
[![Firmware Phase](https://img.shields.io/badge/Firmware-RTOS_Core_Ready-blue)](#)
[![Defence Grade](https://img.shields.io/badge/Category-Defence--Grade-red)](#)

A high-performance, AI-enhanced Power Distribution Board (PDB) powered by the **STM32H743ZIT6** MCU. Designed for autonomous systems requiring deterministic safety, real-time telemetry, and TinyML-based load profiling.

## 🚀 Key Features
- **Deterministic Gating**: 5-rail hardware-enforced power distribution with <1ms safety response.
- **Dual-MCU Architecture**: STM32H7 (Control & Inference) + ESP32 (SCADA & Telemetry).
- **High-Speed Sensing**: DMA-optimized I2C data acquisition from INA219 sensors.
- **TinyML Ready**: Optimized for GNN/LSTM load class inference at the edge.
- **Defence-Grade Design**: MIL-STD-810H thermal management and high-current busbars.

## 📁 Project Structure
- `/hardware`: KiCAD 7.0/8.0 schematics and 4-layer PCB layout.
- `/firmware`: FreeRTOS-based STM32H7 control logic.
- `/scada`: MQTT telemetry gateway and dashboard configurations.
- `/aicore`: Training datasets and edge-inference models.
- `/docs`: Technical specifications and block diagrams.

## 🛠 Quick Start
1. **Hardware**: Open `hardware/SPDB.kicad_pro` to view the 6-sheet hierarchical design.
2. **Firmware**: Import the `firmware/` folder as an STM32CubeIDE project.
3. **Manufacture**: Run `python3 hardware/scripts/gen_gerbers.py` to generate fabrication outputs.

## 🛡 License
Proprietary - Developed for GARUD SYSTEMS Defence Projects.

# FPGA-ARM Image Processing Project

## Project Goal
Build a complete pipeline: **PC Video Input → FPGA Capture/Process → UART → RK3568 ARM → Image Reconstruction**

## Members
- **ARM Side:** adacliff223-alt
- **FPGA Side:** [To be filled]

## Current Status
- ARM side: UART communication framework ready
- FPGA side: Initialization phase
- Main focus: Establishing stable UART protocol communication

## Directory Structure
- `docs/` - Project documentation (protocol, status, debug logs)
- `arm/` - RK3568 ARM-side code and utilities
- `fpga/` - FPGA design and RTL
- `testdata/` - Test data and sample frames
- `tools/` - Helper scripts and utilities

## Quick Start - ARM Demo
```bash
cd arm
python3 main.py
```

## Protocol Overview
See `docs/protocol.md` for detailed UART protocol specification.

- Baud Rate: 115200
- Frame Size: 2058 bytes
- Image Dimensions: 64×32 pixels
- 16-frame mosaic support

## Project Status
For current progress, open issues, and roadmap, see `docs/project_status.md`
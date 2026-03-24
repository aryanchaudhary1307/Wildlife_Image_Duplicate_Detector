# Wildlife_Image_Duplicate_Detector
ASIC implementation of a dHash-based image signature generator for wildlife conservation
# Wildlife Image Duplicate Detector
**Team:** The MOSFET Mob  
**Event:** UnPlugged Hardware Hackathon

## Project Overview
This project implements a hardware-efficient **dHash (Difference Hash)** algorithm in Verilog. It processes 640x480 grayscale streams to detect redundant images, saving storage and power in remote camera traps.

## Key Features
* **Real-time Pipeline:** Processes pixels on-the-fly via line buffers.
* **64-bit Signature:** Uses perceptual hashing for lighting-resilient detection.
* **Resource Optimized:** Designed for Basys 3 (Artix-7) with memory-efficient streaming.

## Repository Structure
* `/src`: RTL source code (Verilog).
* `/sim`: Testbench and simulation results.
* `/docs`: System architecture diagrams and waveforms.

## How to Run
1. Load `src/*.v` into Vivado.
2. Run simulation using `sim/tb_top.v`.
3. Observe the `duplicate_detected` signal at the end of the frame.

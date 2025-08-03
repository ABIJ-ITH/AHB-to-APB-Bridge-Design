# AHB to APB Bridge Design in Verilog

A system to interface **AHB (Advanced High-performance Bus)** with **APB (Advanced Peripheral Bus)**, allowing seamless communication between high-speed and low-speed components in a System-on-Chip (SoC) design.

---

## Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [How It Works](#how-it-works)
- [Schematic](#schematic)
- [Setup Instructions](#setup-instructions)
- [Simulation Results](#simulation-results)
- [License](#license)

---

## About the Project
This project implements an **AHB to APB Bridge** in Verilog for efficient data transfer between two AMBA protocols.  
The bridge handles:
- AHB sequential and non-sequential transfers  
- APB setup and enable phases  
- Read and write transactions  

The design is fully synthesizable and simulated successfully with Verilog testbenches.

---

## Features
- ✅ Supports AHB Non-sequential (NONSEQ) and Sequential (SEQ) transfers  
- ✅ Converts AHB transactions to APB format  
- ✅ Supports read and write operations  
- ✅ Fully synthesizable Verilog design  
- ✅ Functional verification with testbench  

---

## How It Works
1. AHB Master initiates the transaction  
2. Bridge checks transfer type (NONSEQ or SEQ)  
3. Bridge translates signals to APB protocol  
4. APB completes setup and enable phases for peripheral access  
5. Read or write is performed, and response is sent back to AHB  

---

## Schematic
![AHB to APB Bridge Schematic](Screenshots/ahb2apb_schematic.png)

## Setup Instructions
Clone the repository:
```bash
git clone https://github.com/ABIJ-ITH/AHB-to-APB-Bridge-Design.git
```
## Simulation Result
![Simulation Waveform](Screenshots/simulation_waveform.png)

## LISENCE
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

# Digital Techniques 3 – Lab 1 (Project Creation)

## Course
Digital Techniques 3  
University of Oulu

## Lab Overview
This repository contains my work for **Lab 1 – Project Creation**, focusing on the initial setup of the *audioport* system and understanding memory-mapped I/O using the APB bus.

The lab introduces the overall project architecture and serves as the foundation for subsequent verification and RTL design tasks.

## Learning Objectives
- Understand memory-mapped I/O in a SW/HW interface
- Learn APB bus address mapping
- Analyze system-level behavior using a Transaction-Level Model (TLM)
- Understand hierarchical SystemVerilog module integration

## Implemented Work
- Defined APB address map for control and FIFO registers
- Configured design parameters based on student-specific randomizers
- Verified playback start/stop behavior using TLM simulation
- Analyzed interrupt behavior and FIFO refill mechanism
- Verified module connectivity using JasperGold connectivity checks

## Simulation & Verification
- TLM simulations confirm correct command handling (`CMD_START`, `CMD_STOP`)
- FIFO data flow and interrupt behavior match reference model
- All connectivity checks passed with no detected wiring issues

## Notes
Only files **modified by me** are included in this repository.  
Course-provided templates, reference models, and full lab environments are intentionally excluded.

## Disclaimer
This repository is shared for **portfolio and learning demonstration purposes only**.  
Please do not copy this work for academic submissions.

---

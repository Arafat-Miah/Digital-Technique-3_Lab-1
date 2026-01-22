# Digital Technique 3 – Lab 1: Project Setup & System Understanding

## Overview
This repository contains **Lab 1** of the *Digital Technique 3 (DT3)* course.  
The purpose of this lab was to set up the project environment, understand the overall audioport system architecture, define design parameters, and verify the Transaction-Level Model (TLM) behavior before starting RTL implementation.

Lab 1 focuses on **preparation, configuration, and understanding**, not on RTL logic or verification.

---

## Objectives
The main objectives of Lab 1 were:

- Set up the DT3 project environment on Linux
- Understand the audioport system architecture
- Define and verify design parameters consistently across RTL and TLM
- Run and analyze TLM simulations
- Create the top-level RTL module hierarchy
- Verify module connectivity and elaboration

---

## Tasks Completed

### 1. Project and Environment Setup
- Configured the DT3 project workspace
- Reviewed provided documentation and specifications
- Studied APB and audioport architecture basics

---

### 2. Design Parameter Definition
- Defined personal design parameters in:
  - `audioport_pkg.sv` (SystemVerilog)
  - `audioport_defs.h` (SystemC)
- Ensured consistency between RTL and TLM parameter values
- Verified parameters using simulator outputs

---

### 3. APB Bus Configuration
- Defined audioport start and end addresses
- Configured APB input delay and address mapping
- Documented APB-related parameters in the project report

---

### 4. TLM Simulation and Waveform Analysis
- Executed SystemC TLM simulations
- Analyzed waveforms and compared them with reference timing diagrams
- Observed command behavior, play/stop transitions, and IRQ signaling
- Captured waveform screenshots for documentation

---

### 5. RTL Module Hierarchy Creation
- Reviewed module interfaces for:
  - `control_unit`
  - `cdc_unit`
  - `dsp_unit`
  - `i2s_unit`
- Instantiated all submodules in the top-level `audioport` module
- Declared and connected internal signals according to the block diagram

---

### 6. Elaboration and Connectivity Verification
- Successfully compiled and elaborated the RTL design
- Resolved unconnected ports and signal width mismatches
- Verified connectivity using:
  - Simulator schematic inspection
  - Connectivity check tools

---

## Key Learning Outcomes
Through this lab, I learned:

- How a larger hardware project is structured
- The importance of consistent parameter definitions across models
- How to interpret TLM simulations to understand expected RTL behavior
- How to read block diagrams and module specifications
- How to verify RTL connectivity before functional implementation

---

## Notes
- No functional RTL logic or verification code was implemented in this lab
- All work focused on setup, configuration, and understanding
- This lab provides the foundation for later RTL and verification tasks

---

## Next Steps
- Lab 2 focuses on RTL verification of the `control_unit`
- Writing directed tests, assertions, and waveform-based debugging

---

## Author
**Arafat Miah**  
Digital Technique 3 – University of Oulu

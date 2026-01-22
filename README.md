# Digital Technique 3 – Lab 1  
## Project Setup, TLM Simulation, and System Understanding

### Course
Digital Technique 3  
University of Oulu

---

## Lab 1 Overview

This repository documents **Lab 1** of the Digital Technique 3 course.  
The main goal of this lab was to **set up the project environment**, **configure student-specific parameters**, and **understand the behavior of the audioport system** using **Transaction-Level Model (TLM) simulation**.

No new RTL or verification code was written in this lab.  
The focus was on **system bring-up, configuration, simulation, and waveform analysis**.

---

## Objectives of Lab 1

- Set up the DT3 project and simulation environment
- Understand the overall audioport architecture
- Configure numeric parameters and address mapping
- Run TLM-based simulations
- Analyze waveforms and system behavior
- Compare simulation results with specification diagrams

---

## Work Performed

### 1. Project Setup and Configuration
- Configured the DT3 project workspace
- Adjusted student-specific numeric parameters
- Verified correct APB address mapping
- Ensured consistency between SystemVerilog and SystemC models

---

### 2. TLM Simulation
- Executed TLM simulations using QuestaSim
- Observed APB write/read transactions
- Verified command execution (START / STOP)
- Observed data flow through register banks, DSP, and I2S interface

---

### 3. Waveform Analysis
Waveforms were analyzed to confirm correct behavior of:
- Register interface
- Playback control logic
- DSP data flow
- Audio input/output alignment
- I2S signal timing

The screenshots below document the verified behavior.

---

## Simulation Results (Screenshots)

### Screenshot 1 – Register Interface and Playback Control
**File name:** `lab1_register_playback_control.png`

This screenshot shows:
- Register bank activity during APB transactions
- Playback control state transitions (STOP → PLAY)
- Active configuration, level, and DSP registers
- Correct command handling at system level

---

### Screenshot 2 – Audio Input and Output Timing
**File name:** `lab1_audio_in_out_tlm.png`

This screenshot shows:
- TLM audio input signals (left and right channels)
- Corresponding audio output signals
- Correct data propagation through the DSP block
- Alignment between input and output streams

This confirms that the TLM model processes audio data correctly.

---

### Screenshot 3 – I2S Output and DSP Interaction
**File name:** `lab1_i2s_dsp_waveform.png`

This screenshot shows:
- I2S signals (`sck_out`, `ws_out`, `sdo_out`)
- DSP input/output behavior
- Playback state maintained during streaming
- Correct timing relationship between DSP and I2S blocks

---

## Key Learning Outcomes

Through Lab 1, I learned:

- How a complex hardware system is structured and initialized
- The role of TLM models in defining expected RTL behavior
- How APB transactions control system operation
- How to analyze waveforms to verify functional behavior
- Why configuration and system-level understanding are critical before RTL verification

---

## Notes

- No new RTL or testbench code was written in this lab
- All work focused on configuration, simulation, and analysis
- Screenshots are included to demonstrate verified system behavior
- Course-provided reference code is not modified or redistributed

---

## Next Steps

- Lab 2 focuses on writing SystemVerilog test tasks and assertions
- RTL verification of the control unit is performed in later labs

---

## Disclaimer

This repository is shared for **learning and portfolio demonstration purposes only**.  
Please do not reuse this content for academic submissions.

---

## Author

**Arafat Miah**

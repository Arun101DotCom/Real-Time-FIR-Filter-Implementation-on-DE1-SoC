# Real-Time-FIR-Filter-Implementation-on-DE1-SoC
This project involved designing a real-time FIR Low-Pass Filter on a Terasic DE1-SoC FPGA using VHDL. I developed core modules for I2C/I2S codec initialization and serial-to-parallel conversion. Validated via Quartus Prime and Questa simulations, the system was hardware-tested with a 1–30kHz sweep to analyze frequency response and cut-off ranges.


## Project Description
This project focuses on the design and implementation of a Finite Impulse Response (FIR) digital filter.

The system is built on the Terasic DE1-SoC development board using an Intel Cyclone V FPGA.

All hardware logic is written in VHDL to provide high-speed, parallel processing of audio signals.

The design allows for real-time filtering of audio input with a specific cut-off frequency range.

## Academic and Technical Objectives
Gain expertise in reconfigurable hardware and FPGA design flows.

Implement a complete digital system using VHDL and IEEE 1076-1993 libraries.

Master communication protocols for audio codecs, specifically I2C and I2S.

Compare the performance and energy efficiency of HDL against software platforms like C and Java.

## System Components
Codec Initialization: Configures the audio chip via I2C for proper input/output operation.

S2P Adapter: Converts Serial audio data to Parallel words for processing in the FPGA.

FIR Filter Block: Executes the mathematical filtering algorithm using Multiply-Accumulate logic.

Data Tracking: Uses ADCstb and DACstb signals to synchronize data between blocks.

## Verification and Testing
Software Simulation: Tested all .vhd files in Questa-Intel FPGA Edition and ModelSim.

Waveform Analysis: Validated shift registers, bit counters, and word counters through timing diagrams.

Hardware Implementation: Programmed the Cyclone V chip using the Quartus Prime Programmer.

Real-Time Analysis: Used a signal generator to sweep frequencies from 1 kHz to 30 kHz.

Final Result: Plotted the frequency response curve using an Oscilloscope to confirm the low-pass behavior.

## Tools Used
Quartus Prime Lite Edition 23.1 for synthesis and pin assignment.

Questa-Intel FPGA / ModelSim for VHDL simulation and verification.

Terasic DE1-SoC Board for physical hardware execution.

Standard Lab Equipment including a Function Generator and Digital Oscilloscope.

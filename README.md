# 🚀 Real-Time-FIR-Filter-Implementation-on-DE1-SoC  

Design and Implementation of a Real-Time FIR Low-Pass Digital Filter on FPGA using VHDL  
**Program:** MSc in Electrical & Electronic Engineering  
**Domain:** FPGA-Based Digital Signal Processing (DSP)

---

## 🔬 Project Overview
* This project focuses on the **design, implementation, and real-time validation** of a **Finite Impulse Response (FIR) Low-Pass Filter**
* Implemented on the **Terasic DE1-SoC development board** using an **Intel Cyclone V FPGA**
* All hardware logic is written entirely in **VHDL**
* The system integrates:
  * **Audio codec initialization (`I2C`)**
  * **Serial audio communication (`I2S`)**
  * **Serial-to-parallel data conversion**
  * **Multiply–Accumulate (MAC)-based FIR filter architecture**
* Verified through **simulation** and **hardware testing**
* Tested using a **1–30 kHz frequency sweep**

---

## 🎯 Academic & Technical Objectives
* Gain expertise in **reconfigurable computing** and FPGA-based DSP systems
* Implement a complete digital audio processing pipeline using **VHDL (IEEE 1076-1993)**
* Master **`I2C`** and **`I2S`** communication protocols
* Perform **simulation-driven verification** prior to hardware deployment
* Compare **HDL-based processing efficiency** with software approaches (`C`, `Java`)

---

## 🛠️ System Architecture

### 🔧 1. Codec Initialization Module (`I2C`)
* Configures the onboard audio codec
* Sets sampling frequency, word length, and audio routing paths

### 🔁 2. Serial-to-Parallel Adapter (`I2S`)
* Converts incoming **serial audio streams** into parallel words
* Synchronizes data using bit clock and word select signals

### 🧮 3. FIR Filter Core
* Implements the **low-pass FIR filtering algorithm**
* Uses **Multiply–Accumulate (MAC)** logic for real-time computation

### ⏱️ 4. Data Tracking & Synchronization
* Uses control signals such as `ADCstb` and `DACstb`
* Ensures precise timing alignment between processing stages

---

## 🧪 Verification & Testing

### 🖥️ Software Simulation
* Simulated all `.vhd` files using:
  * **Questa-Intel FPGA Edition**
  * **ModelSim**
* Verified logic correctness and timing behavior

### 📈 Waveform Analysis
* Validated:
  * Shift registers
  * Bit counters
  * Word counters
* Analyzed timing diagrams for protocol compliance

### 💾 Hardware Implementation
* Synthesized and programmed the design onto the **Cyclone V FPGA**
* Used **Quartus Prime Programmer**

### 🎛️ Real-Time Frequency Analysis
* Applied a **1 kHz – 30 kHz frequency sweep**
* Observed filtered output using a **digital oscilloscope**
* Confirmed:
  * Passband response
  * Cut-off frequency range
  * High-frequency attenuation

---

## 🏆 Key Outcomes
* Successful **real-time FIR low-pass filter implementation** on FPGA
* Stable audio processing using **`I2C` / `I2S` protocols**
* Verified **low-pass frequency response** through hardware testing
* Demonstrated deterministic and efficient **HDL-based DSP performance**

---

## 🧰 Tools & Technologies
* **Quartus Prime Lite Edition 23.1**
* **Questa-Intel FPGA / ModelSim**
* **Terasic DE1-SoC Board**
* Function Generator
* Digital Oscilloscope

---

## 📂 Repository Structure

* **01_Technical Report
* **02_Sourse Code
* **03_Output Data



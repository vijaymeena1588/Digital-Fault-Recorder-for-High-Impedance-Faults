# Digital Fault Recorder for High Impedance Faults

An **Arduino-based Digital Fault Recorder (DFR)** system for monitoring 230V AC power lines and detecting **high-impedance faults (HIFs)** using hardware and machine learning.

## Overview

This project integrates hardware and software to monitor electrical waveforms, extract key features, and classify subtle faults that traditional systems might miss. It enhances **power system reliability and safety** by providing real-time alerts and fault detection.

## Features

- **Hardware System:** Arduino-based DFR with voltage sensors for 230V AC waveform acquisition.  
- **Signal Processing:** RMS calculation, harmonic monitoring at 2 kHz, and feature extraction.  
- **Display & Alerts:** OLED display shows live voltage and RMS values, with alert logic for abnormal arcing.  
- **Machine Learning:** Classifies extracted features to detect subtle high-impedance faults.  

## Hardware Requirements

- Arduino Uno or compatible board  
- Voltage sensors (for 230V AC measurement)  
- OLED display  
- Signal conditioning circuitry  
- Connecting wires and breadboard/PCB  

## Software Requirements

- Arduino IDE  
- Python (for ML model training and testing)  
- Required Python libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`  

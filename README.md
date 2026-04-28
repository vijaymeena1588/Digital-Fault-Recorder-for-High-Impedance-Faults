# Digital Fault Recorder for High Impedance Faults

An **Arduino-based Digital Fault Recorder (DFR)** for detecting **High Impedance Arcing Faults (HIAF)** through spectral analysis and real-time signal monitoring. The system combines low-cost hardware with advanced signal processing to identify non-linear arcing signatures in power systems.

---

## Overview

This project integrates custom-built hardware and a Python-based analysis engine to:

- Acquire conditioned voltage waveforms at **20 kHz sampling**
- Perform **FFT + Power Spectral Density (PSD)** analysis
- Detect characteristic HIF signatures such as:
  - Fundamental power collapse (>30%)
  - Rise in odd-order harmonics (3rd, 5th)
  - Elevated broadband noise (200–500 Hz band)
- Generate real-time fault alerts

The setup was experimentally validated under **10–30 kV laboratory conditions** using a tree-leaning fault model.

---

## Key Features

- **Low-Cost Hardware (< INR 800):**  
  Arduino-based DFR with signal conditioning for safe waveform acquisition.

- **High-Resolution Sampling:**  
  20 kHz sampling frequency for capturing arc-induced high-frequency components.

- **Spectral Fault Detection Logic:**  
  - 3rd harmonic (150 Hz) PSD > 5%  
  - 5th harmonic (250 Hz) PSD > 3%  
  - 200–500 Hz broadband energy > 2.5%  
  - Fundamental energy collapse > 30%

- **Automated Python Analysis Engine:**  
  Real-time FFT, PSD computation, harmonic tracking, and alert generation.

- **Live Monitoring Output Example:**

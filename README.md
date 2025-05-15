# OFDM Voice Transmission Simulator

This project simulates a wireless communication system using **Orthogonal Frequency Division Multiplexing (OFDM)** and **64-QAM** modulation for transmitting a voice signal through a **frequency-selective fading channel**. It is implemented in MATLAB as a single Live Script file: `mcom_project.mlx`.

---

## 📁 File Overview

- **`mcom_project.mlx`** – MATLAB Live Script containing the full implementation of the simulator including:
  - Voice recording and conversion to bitstream
  - 64-QAM modulation and demodulation
  - OFDM modulation and demodulation with cyclic prefix
  - Channel simulation with multipath fading and AWGN
  - Receiver-side processing and audio reconstruction
  - Performance metrics and visualization plots

---

## 🚀 How to Run the Simulator

1. Open MATLAB.
2. Navigate to the folder containing `mcom_project.mlx`.
3. Open the file and click **Run Section** step-by-step to observe outputs.
4. You will be prompted for several optional inputs during runtime (e.g., Emin, sampling frequency, noise PSD).

---

## 🧾 User Inputs (with defaults if skipped)

- **Emin** (energy of closest constellation point): `1e-15`
- **Sampling frequency (Hz)**: `1e6` (1 MHz)
- **Number of multipath components**: `4`
- **Path delays (µs)**: `[0, 5, 10, 15]`
- **Noise PSD (W/Hz)**: `1e-9`

---

## 📊 Outputs

- Bit Error Rate (BER) and Symbol Error Rate (SER)
- Constellation diagrams:
  - Transmitted (64-QAM)
  - Received (before and after equalization)
- Channel impulse response plot (in dBW)
- Reconstructed audio playback and waveform comparison

---

## ✅ Features Implemented

- End-to-end simulation from voice to playback
- 64-QAM and OFDM processing
- Frequency-selective multipath fading using sum-of-sinusoids (no inbuilt MATLAB fading channel functions)
- AWGN noise modeling
- OFDM equalization using frequency domain techniques

---

## 📄 Reference

This simulator was developed as part of the **MCOM 2025 (ECE 343)** course project based on the problem described in `mcom.pdf`. The theoretical background, results, and observations are detailed in `MCOM Project Report.pdf`.

---



# 🌞 Time Series Decomposition for Enhanced Solar Flare Forecasting

This repository supports the paper:

**"Time Series Decomposition Using Wavelet and Fourier Transforms for Enhanced Solar Flare Forecasting"**  
Victor Solomon, Omkar Rayala, Manya Rampuria, Abdul Afrid, Junzhi Wen, Rafal Angryk  
Department of Computer Science, Georgia State University

---

## 🔍 Overview

This project investigates how frequency-based time series decomposition can improve multivariate solar flare prediction. We apply four transformation methods:

- **Haar Wavelet Transform (HWT)**
- **Symlet Wavelet Transform (SWT)**
- **Daubechies Wavelet Transform (DWT)**
- **Discrete Fourier Transform (DFT)**

We evaluate the effectiveness of these transforms on both **lossless** and **lossy** time series reconstructions using two classifiers:

- **Time Series Forest (TSF)** for time series data
- **Random Forest (RF)** for decomposed, non-time-series (NTS) data

---

## 🧪 Experiments

### ✅ Experiment I: TS Reconstruction Impact
We assess the performance of TSF trained on:
- Original data
- Lossless reconstructed data
- Lossy reconstructed data (based on 20dB SNR filtering)

📊 Metrics: **TSS** and **HSS2**

### ✅ Experiment II: TS vs NTS Representations
We compare:
- TSF (trained on full and reduced TS)
- RF (trained on decomposed NTS)

🕒 Time windows tested: 720, 320, 96, and 48 minutes (60, 30, 8, 4 timepoints respectively)

---

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/solar-flare-decomposition.git
   cd solar-flare-decomposition

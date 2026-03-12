
# ECG HRV Pipeline

A Python pipeline for ECG signal processing and Heart Rate Variability (HRV) 
analysis, independently developed as part of a self-directed learning journey 
in computational neuroscience and biosignal analysis.

---

## 🎯 Project Goal

To understand and implement a complete HRV analysis pipeline from scratch — 
starting from simulated ECG signals, progressing to real ECG data from PhysioNet, 
detecting R peaks, computing R-R intervals, and calculating both time domain 
(SDNN, RMSSD) and frequency domain (LF, HF, LF/HF ratio) HRV metrics.

This project is a foundation for a larger analysis of HRV during slow-paced 
breathing at 0.1 Hz (resonance frequency), which is being developed in a 
[separate repository](https://github.com/aishwarya-dangat/hrv-slow-breathing).

---

## 🧠 What is HRV?

Heart Rate Variability (HRV) measures the variation in time between consecutive heartbeats (R-R intervals). The heart does not beat like a metronome — it naturally speeds up and slows down. This variability reflects the activity of the autonomic nervous system and is widely used as a marker of stress, recovery, and cardiovascular health.

---

## 📊 What This Notebook Does

- Simulates a realistic ECG signal using NeuroKit2 (60 seconds, 1000 Hz sampling rate)
- Visualises the raw ECG signal
- Automatically detects R peaks using NeuroKit2's ECG processing pipeline
- Extracts R-R intervals using NumPy
- Computes two standard HRV metrics:
  - **SDNN** — standard deviation of R-R intervals (overall variability)
  - **RMSSD** — root mean square of successive differences (short-term variability)
- Visualises R-R intervals over time with mean reference line
- - Loads real ECG data from PhysioNet MIT-BIH Database using WFDB
- Detects R peaks and computes R-R intervals from real data
- Computes time domain metrics (SDNN, RMSSD) on real data
- Computes frequency domain metrics (LF, HF, LF/HF ratio) using scipy
- Visualises HRV power spectrum with LF/HF bands and 0.1 Hz marker

---

## 🛠️ Tools & Libraries

- Python 3
- [NeuroKit2](https://neurokit2.readthedocs.io/) — biosignal processing
- NumPy — numerical computation
- Matplotlib — visualisation
- scipy — frequency domain signal processing
- WFDB — loading PhysioNet ECG recordings

---

## 📁 Files

- `ecg_hrv_pipeline.ipynb` — Main analysis notebook (Google Colab compatible)
- hrv_analysis_real_data.ipynb
---

## 🔬 Status

✅ Simulated ECG pipeline complete
✅ Real ECG data loaded from PhysioNet (MIT-BIH Database)
✅ Time domain metrics (SDNN, RMSSD) computed
✅ Frequency domain metrics (LF, HF, LF/HF ratio) computed
✅ HRV Power Spectrum visualised
---

## 👩‍🔬 Author

**Aishwarya S. Dangat**  
Cognitive Neuroscientist, MSc — Sapienza University of Rome  
Independently learning computational neuroscience methods for biosignal analysis.

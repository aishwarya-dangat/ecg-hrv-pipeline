# ecg-hrv-pipeline
ECG signal processing and HRV metric extraction using NeuroKit2 and NumPy
# ECG HRV Pipeline

A beginner-friendly Python pipeline for ECG signal processing and Heart Rate Variability (HRV) analysis, built independently as part of an ongoing learning journey in computational neuroscience.

---

## 🎯 Project Goal

To understand and implement the fundamentals of HRV analysis from scratch — starting from simulated ECG signals, detecting R peaks, computing R-R intervals, and calculating standard HRV metrics.

This project is a foundation for a larger analysis of HRV during slow-paced breathing at 0.1 Hz (resonance frequency), which is being developed in a [separate repository](https://github.com/aishwarya-dangat/hrv-slow-breathing).

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

---

## 🛠️ Tools & Libraries

- Python 3
- [NeuroKit2](https://neurokit2.readthedocs.io/) — biosignal processing
- NumPy — numerical computation
- Matplotlib — visualisation

---

## 📁 Files

- `ecg_hrv_pipeline.ipynb` — Main analysis notebook (Google Colab compatible)

---

## 🔬 Status

✅ Simulated ECG pipeline complete  
🔄 Real dataset integration — in progress  
🔄 Slow breathing (0.1 Hz) condition analysis — in progress  
🔄 Frequency domain metrics (LF, HF, LF/HF ratio) — planned  

---

## 👩‍🔬 Author

**Aishwarya S. Dangat**  
Cognitive Neuroscientist, MSc — Sapienza University of Rome  
Independently learning computational neuroscience methods for biosignal analysis.

# EEG-Motor-Imagery-Classification-for-Brain-Computer-Interface-Using-Spectral-Features
# EEG Motor Imagery Classification for BCI

This project implements a Brain-Computer Interface (BCI) pipeline to classify motor imagery (left vs right hand movement) using EEG signals and Digital Signal Processing techniques.

## 🧠 Overview

A Brain-Computer Interface (BCI) enables direct communication between the brain and external devices. This project uses EEG signals and spectral features to classify motor imagery tasks.

We use:
- EEG dataset from PhysioNet
- Signal processing (bandpass filtering)
- FFT for feature extraction
- KNN for classification

---

## ⚙️ Pipeline

1. Load EEG data using MNE
2. Apply bandpass filter (8–30 Hz)
3. Extract epochs (0–2 sec)
4. Compute FFT for each channel
5. Extract mean spectral power
6. Train KNN classifier (k=3)
7. Evaluate using accuracy & confusion matrix

---

## 📊 Results

- Dataset: 15 trials (Subject 1)
- Accuracy: **20%**
- Issue: Small dataset + simple features

---

## 📉 Limitations

- Very small dataset
- Basic feature extraction (mean FFT)
- No artifact removal
- No cross-subject validation

---

## 🚀 Future Improvements

- Use Common Spatial Patterns (CSP)
- Separate alpha & beta band power
- Apply ICA for noise removal
- Use deep learning models (EEGNet)

---

## 📦 Installation

```bash
pip install -r requirements.txt

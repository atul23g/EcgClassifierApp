# ECG Classifier App

This repository contains a complete project that classifies ECG (Electrocardiogram) signals to detect different heart conditions. It includes:

- **Android app**: An app built with Android Studio to upload ECG images and get predictions.
- **Python code**: Scripts to process data and interact with the machine learning model.
- **Model training code**: `ecg_classifier.py` contains the Python code to train the machine learning model used for ECG classification.

---

## How the parts work together

1. The **model training script (`ecg_classifier.py`)** trains a machine learning model on ECG data and saves the trained model (`ecg_model.pkl`).

2. The **Python backend** loads this trained model and exposes a prediction API (for example, using Flask). It takes ECG images or data as input and returns predictions.

3. The **Android app** allows users to select ECG images and sends them to the backend API to get predictions, which are then displayed in a user-friendly way.

---

## How to use this project

### 1. Train the model (optional)

If you want to train your own model or improve it, run:

```bash
python python-code/ecg_classifier.py

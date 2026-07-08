# EEG-Based Mental Stress Detection Using Deep Learning

## Overview

This project presents a deep learning-based approach for mental stress detection using Electroencephalography (EEG) signals. Instead of directly using raw EEG time-series data, the signals are transformed into frequency-band topographic grid representations that preserve the spatial distribution of brain activity. These representations are then used to train Convolutional Neural Networks (CNNs) for binary stress classification.

The proposed approach combines EEG signal preprocessing, frequency-domain feature extraction, topographic image generation, and deep learning to achieve accurate mental stress detection.

---

## Dataset

**STEW (Simultaneous Task EEG Workload) Dataset**

* 48 subjects
* 14-channel EEG recordings
* Sampling frequency: 128 Hz
* Binary classification:

  * Low Stress
  * High Stress

---

## Features

* EEG signal preprocessing
* Frequency-band extraction
* Band-pass filtering
* Topographic grid generation
* CNN-based stress classification
* Model evaluation using multiple performance metrics
* IEEE conference paper accepted based on this work

---

## Methodology

1. Load EEG recordings from the STEW dataset.
2. Apply preprocessing and filtering.
3. Extract frequency bands:

   * Delta (1–4 Hz)
   * Theta (4–8 Hz)
   * Alpha (8–13 Hz)
   * Beta (13–30 Hz)
   * Gamma (30–45 Hz)
4. Generate topographic grid representations for each frequency band.
5. Train a Convolutional Neural Network on the generated images.
6. Evaluate model performance using standard classification metrics.

---

## Technology Stack

* Python
* PyTorch
* OpenCV
* NumPy
* Pandas
* MNE
* Matplotlib
* Scikit-learn

---

## Results

The proposed model achieved over **90% classification accuracy** on the STEW dataset.

Evaluation metrics include:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## Topographic Grid Examples

<img width="623" height="122" alt="image" src="https://github.com/user-attachments/assets/fcdd16f9-4c18-4cbb-94bd-6afe34119f42" />


---

## Project Structure

```text
EEG-Stress-Detection/
│── dataset/
│── preprocessing/
│── topographic_generation/
│── models/
│── training/
│── evaluation/
│── results/
│── images/
│── requirements.txt
└── README.md
```

---

## Future Improvements

* Vision Transformer (ViT)-based classification
* Subject-independent evaluation
* Real-time EEG stress detection
* Explainable AI (Grad-CAM)
* Multi-class stress level prediction
* Deployment as a web application

---

## Publication

**Accepted for Presentation**

**IEEE International Conference on Sustainability, Innovation and Technology (ICSIT 2026)**

**Paper Title:**

*Mental Stress Detection Using EEG Signals Based on Frequency-Band Topographic Grid Representation and Deep Convolutional Neural Networks*

---

## Installation

Clone the repository:

```bash
git clone https://github.com/VardhanVelamakanni/EEG-Stress-Detection.git
cd EEG-Stress-Detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run training:

```bash
python train.py
```

Run evaluation:

```bash
python evaluate.py
```

---

## Author

**Hemavardhan Velamakanni**

Computer Vision | Deep Learning | Machine Learning

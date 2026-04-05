# Automated Infant Cry Classification using Deep Learning

## 📌 Overview

This project presents an automated system for classifying infant cry sounds into meaningful categories using audio signal processing and machine learning techniques. The system analyzes cry audio and predicts the underlying reason, aiding caregivers in understanding infant needs more effectively.

---

## 🎯 Problem Statement

Infant crying is the primary mode of communication, but interpreting its cause (such as hunger, discomfort, or fatigue) is challenging. This project aims to develop a reliable classification system that can automatically identify the reason behind a baby’s cry using audio-based analysis.

---

## 📂 Dataset

* **Source:** Kaggle Baby Cry Sounds Dataset
* **Classes:**

  * belly pain
  * burping
  * cold_hot
  * discomfort
  * hungry
  * laugh
  * silence
  * tired

📎 Dataset link: https://www.kaggle.com/datasets/mennaahmed23/baby-cry-sounds

> Note: Dataset is not included in this repository due to size constraints.

---

## ⚙️ Methodology

### 1. Audio Preprocessing

* Silence trimming
* Resampling
* Normalization

### 2. Data Augmentation

* Noise injection
* Time stretching
* Pitch shifting

### 3. Feature Extraction

* MFCC
* MFCC + Delta features
* Log-Mel Spectrogram

---

## 🤖 Models Used

### 🔹 Classical Machine Learning

* Random Forest
* Support Vector Machine (SVM)
* XGBoost

### 🔹 AutoML

* AutoGluon
* H2O AutoML
* TPOT

### 🔹 Deep Learning (Proposed Model)

* ResNet-18 (Transfer Learning on Log-Mel Spectrograms)

---

## 📊 Results

| Model                | Accuracy   |
| -------------------- | ---------- |
| Random Forest        | ~44%       |
| SVM                  | ~49%       |
| XGBoost              | ~44%       |
| AutoGluon            | ~52%       |
| TPOT                 | ~54%       |
| ResNet-18 (Proposed) | **53.37%** |

* **Macro F1 Score (ResNet-18): 0.5983**
* ResNet-18 demonstrated better generalization and improved handling of class imbalance.

---

## 🚀 Key Highlights

* Comparative study of Classical ML, AutoML, and Deep Learning approaches
* Use of audio signal processing techniques for feature extraction
* Implementation of transfer learning with ResNet-18
* Ensemble-based prediction for improved performance

---

## ▶️ How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/infant-cry-classification.git
cd infant-cry-classification
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Run the notebooks:

* `babycry_analysis.ipynb`
* `babycry(new).ipynb`

---

## 📦 Requirements

* Python 3.x
* numpy
* pandas
* librosa
* scikit-learn
* torch
* matplotlib

---

## 🔮 Future Work

* Increase dataset size and diversity
* Explore transformer-based audio models
* Deploy as a real-time application
* Integrate explainable AI for better interpretability

---

## 👩‍💻 Developed By

Shreejaa S M

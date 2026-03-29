#  Plant Disease Detector AI

> Intelligent plant disease detection system built with Deep Learning: MobileNetV2 Transfer Learning, plus Grad-CAM for clear visual explanations.
![Python](https://img.shields.io/badge/Python-3.11-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-orange)
![Accuracy](https://img.shields.io/badge/Accuracy-87%25-green)
![License](https://img.shields.io/badge/License-MIT-purple)

---

## Overview

This project implements an intelligent system for automatic detection of plant leaf diseases using Convolutional Neural Networks and Transfer Learning. Trained on the PlantVillage dataset, the model classifies leaf images into 15 disease categories with over 87% validation accuracy.

The system integrates Grad-CAM visual explanations to highlight infected regions — making the AI decision interpretable and trustworthy for real-world agricultural use.

---

## Problem Statement

Plant diseases destroy between 20% and 40% of global crops annually. Manual detection by agronomists is slow, expensive, and inaccessible to small-scale farmers. This system provides an automated, fast, and accessible alternative : a farmer only needs a photo of a leaf.

---

##  Technical Approach

| Component | Choice | Reason |
|-----------|--------|--------|
| Base model | MobileNetV2 | Lightweight, deployable on embedded systems |
| Training strategy | Transfer Learning | 87%+ accuracy with limited data |
| Explainability | Grad-CAM | Visualizes infected leaf regions |
| Interface | Streamlit | Python-native web app |
| Dataset | PlantVillage | 41,273 images, 15 classes |

---

## Dataset

- **Source** : PlantVillage Dataset (Mohanty et al., 2016)
- **Total images** : 41,273
- **Classes** : 15 (diseases + healthy)
- **Plants covered** : Tomato, Potato, Pepper bell
- **Split** : 80% train / 20% validation

---

##  Project Structure
```
plant-disease-detector/
├── data/                  # PlantVillage dataset
├── models/                # Trained models (.h5, .tflite)
├── notebooks/             # Jupyter notebooks
│   ├── 01_dataset_exploration.ipynb
│   └── 02_preprocessing_model.ipynb
├── src/                   # Python modules
├── results/               # Graphs, confusion matrix
│   ├── dataset_samples.png
│   └── class_distribution.png
├── docs/                  # Documentation
├── requirements.txt
└── README.md
```

---

##  Results

| Metric | Value |
|--------|-------|
| Validation Accuracy | **87%+** |
| Training Epochs | 20 (Early Stopping) |
| Model Size | ~9 MB |
| Inference Time | < 1 second |

---

##  Scientific References

- Mohanty, S.P., Hughes, D.P., & Salathé, M. (2016). *Using Deep Learning for Image-Based Plant Disease Detection*. Frontiers in Plant Science.
- Selvaraju, R.R., et al. (2017). *Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization*. ICCV.
- Howard, A.G., et al. (2018). *MobileNetV2: Inverted Residuals and Linear Bottlenecks*. CVPR.

---

##  Author

**Malek AL-Jebali**  
IoT & Embedded Systems Engineering Student — ISTIC Borj Cedria, Tunisia  
[GitHub](https://github.com/dr-aljebalimk)

---

##  License

MIT License — feel free to use and build upon this work.

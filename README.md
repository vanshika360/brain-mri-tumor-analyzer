# 🧠 Brain MRI Tumor Analyzer

> **Deep Learning-based Brain Tumor Detection & Segmentation**  
> Classification: **85.8% Accuracy** | Segmentation: **86.7% Dice Score**

[![Live Demo](https://img.shields.io/badge/🤗%20Live%20Demo-Hugging%20Face-yellow)](https://huggingface.co/spaces/Vanshika250/Brain-mri-analyzer)
[![Python](https://img.shields.io/badge/Python-3.8+-blue)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://tensorflow.org)
[![Gradio](https://img.shields.io/badge/Gradio-App-green)](https://gradio.app)

---

## 📌 Overview

This project implements a **two-stage deep learning pipeline** for brain MRI analysis:

1. **Tumor Classification** — Identifies tumor type using EfficientNetB3
2. **Tumor Segmentation** — Localizes tumor region using a custom U-Net

Upload any brain MRI scan and get instant predictions with tumor type, confidence score, and segmentation mask.

---

## 🚀 Live Demo

👉 **Try it here:** [huggingface.co/spaces/Vanshika250/Brain-mri-analyzer](https://huggingface.co/spaces/Vanshika250/Brain-mri-analyzer)

---

## 🏆 Results

### Classification (EfficientNetB3)

| Class | Recall |
|-------|--------|
| Glioma | 56% |
| Meningioma | 94% |
| No Tumor | 97% |
| Pituitary | 97% |
| **Overall Accuracy** | **85.8%** |

### Confusion Matrix
![Confusion Matrix](images/confusion_matrix.png)

---

### Segmentation (U-Net)

| Metric | Score |
|--------|-------|
| Dice Score | **86.71%** |
| Parameters | 31.4M |

### U-Net Predictions
![U-Net Predictions](images/unet_predictions.png)

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| Classification Model | EfficientNetB3 + Focal Loss |
| Segmentation Model | Custom U-Net (BCE + Dice Loss) |
| Preprocessing | CLAHE contrast enhancement |
| Framework | TensorFlow 2.x |
| Web App | Gradio |
| Deployment | Hugging Face Spaces |

---

## 📁 Project Structure

# Automatic Number Plate Recognition in Adverse Environmental Conditions using Hybrid Deep Learning Models

**Undergraduate Thesis Project**  
**Varendra University** | Department of Computer Science and Engineering

---

## 📋 Project Overview

This research aims to improve **Automatic Number Plate Recognition (ANPR)** accuracy in challenging real-world conditions such as **rain, fog, dust, glare, low illumination, and blur** — which are very common in Bangladesh.

We propose a **Hybrid Deep Learning Model** combining **Convolutional Neural Networks (CNN)** for local feature extraction and **Vision Transformer (ViT)** for global context understanding to achieve better robustness in adverse environments.

---

## 🎯 Objectives

- Develop a robust ANPR system for adverse environmental conditions
- Create and augment a dataset simulating real-world challenges (rain, fog, blur, low light, etc.)
- Design a **Hybrid CNN + Vision Transformer** model for better accuracy
- Compare performance with baseline models (YOLOv8)
- Optimize the model for low-resource edge devices

---

## 📁 Project Structure

Thesis_ANPR/
├── dataset/
│ └── split_anpr/
│ ├── train/
│ │ ├── images/
│ │ └── labels/
│ └── val/
│ ├── images/
│ └── labels/
├── models/
│ ├── yolov8n_baseline_best.pt
│ └── predictions_baseline/
├── cropped_plates_test/
├── runs/ # YOLO training results
├── notebooks/ # Colab notebooks
│ ├── 01_data_preparation.ipynb
│ ├── 02_training_baseline.ipynb
│ ├── 03_augmentation.ipynb
│ └── 04_vit_recognition.ipynb
├── requirements.txt
└── README.md

---

## 🛠️ Technologies Used

- **Detection**: YOLOv8 (Ultralytics)
- **Recognition**: Vision Transformer (ViT) + BanglaBERT (Hybrid Model)
- **Augmentation**: Albumentations
- **Framework**: PyTorch, TensorFlow
- **Tools**: Google Colab, OpenCV, Hugging Face Transformers

---

## 📊 Current Results (Baseline)

- **Model**: YOLOv8n
- **mAP50**: 0.993
- **mAP50-95**: 0.612
- **Precision**: 0.98
- **Recall**: 0.975

The baseline model shows excellent plate detection capability but needs improvement in adverse conditions and character recognition.

---

## 🚀 Future Work

- Strong data augmentation for adverse weather conditions
- Fine-tuning of **ViT + BanglaBERT** for Bangla license plate recognition
- Performance comparison between baseline and hybrid model
- Deployment on edge devices (Jetson Nano / Raspberry Pi)
- Real-time testing in actual Bangladeshi traffic scenarios

---

## 👥 Team Members

- Md. Borhan Uddin Ashik (Me)
- MD MAHEDI HASAN
- AFIA AKHTER

**Supervisor**: Md. Mahfujur Rahman  
**Varendra University**, Department of CSE

---

## 📄 Thesis Documents

- [Thesis Proposal](./Thesis_Proposal.pdf) (now not available)
- [Presentation Slides](./presentation.pdf)

---

## 📞 Contact

- **Email**: [223311161@vu.edu.bd]
- **GitHub**: [github.com/arburhan]

---

**Made with ❤️ for smarter traffic management in Bangladesh**

# Bangladeshi ANPR - Adverse Conditions

**Automatic Number Plate Recognition in Adverse Environmental Conditions using Hybrid Deep Learning Models**

Undergraduate Thesis Project  
**Varendra University**, Department of Computer Science and Engineering

---

## 📋 Project Overview

This project aims to build a robust **ANPR system** that performs well in challenging Bangladeshi weather conditions such as **rain, fog, blur, glare, low light, and dust**.

**Main Contribution**:  
Hybrid **CNN + Vision Transformer (ViT)** model combined with **BanglaBERT** for accurate Bangla license plate recognition.

---

## 📁 Project Structure

```
ANPR/
├── README.md
├── requirements.txt
├── notebooks/                          # All Colab notebooks
│   ├── 01_Data_Split_and_YAML.ipynb
│   ├── 02_YOLOv8_Baseline_Training.ipynb
│   ├── 03_Data_Augmentation.ipynb
│   ├── 04_Plate_Cropping.ipynb
│   └── 05_ViT_BanglaBERT_Recognition.ipynb
├── dataset/
│   └── split_anpr/                    # Train & Val split
│       ├── data.yaml
│       ├── train/
│       │   ├── images/
│       │   └── labels/
│       └── val/
│           ├── images/
│           └── labels/
├── models/                             # Trained YOLOv8 weights
│   ├── yolov8n_baseline_best.pt
│   └── predictions_baseline/
├── cropped_plates/                     # Cropped license plates
│   └── (cropped images)
├── src/                                # Python scripts
│   └── augmentation.py
└── results/                            # Prediction outputs & graphs
    └── (graphs, confusion matrix, etc.)
```

## 🛠️ Technologies & Methods

- **Detection**: YOLOv8n (Ultralytics)
- **Augmentation**: Albumentations (Rain, Fog, Blur, Glare, Low Light)
- **Recognition**: Hybrid **ViT (Encoder) + BanglaBERT (Decoder)**
- **Framework**: PyTorch, Hugging Face Transformers
- **Environment**: Google Colab (GPU)

## 📊 Current Progress

- ✅ Dataset split & YAML configuration
- ✅ YOLOv8n Baseline Training completed
  - mAP50: **0.993**
  - mAP50-95: **0.612**
- ✅ Plate detection & cropping pipeline
- ✅ Initial ViT + BanglaBERT testing (in progress)
- ⏳ Adverse condition augmentation
- ⏳ Full Hybrid Model Fine-tuning

## 📚 Datasets Used

- **Main Dataset**: [Bangladeshi Number Plate - Rajshahi City](https://www.kaggle.com/datasets/mdborhanuddinashik/bangladeshi-number-platte-rajshahi-city)
- **Additional Dataset**: [Bangladeshi Vehicle License Plate](https://www.kaggle.com/datasets/sifatkhan69/bangladeshi-vehicle-license-plate)

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/arburhan/ANPR.git
   ```

# 🏛️ HeritageCracks Dataset: Superficial Damage in Historical Monuments 🏛️

## 📋 Table of Contents
- [Overview](#-overview)
- [Key Features](#-key-features)
- [Dataset Description](#-dataset-description)
- [Dataset Preprocessing & Augmentation](#-dataset-preprocessing--augmentation)
- [Supported Frameworks](#-supported-frameworks)
- [Project Architecture](#-project-architecture)
- [Research Team](#-research-team)
- [License](#-license)

## 📌 Overview
The **HeritageCracks** dataset is a comprehensive collection of images designed to characterize superficial damage in historical monuments within the city of Morelia, primarily focusing on temples. This dataset enables the automated detection and classification of structural deterioration using computer vision and deep learning techniques, contributing to the preservation and structural health monitoring of cultural heritage.

<div align="center">
  <img src="CRACKS_PHONE.v2/train/images/IMG20250330170631_jpg.rf.61d28cf3f04f57611e41c9f2c36061d6.jpg" alt="HeritageCracks Dataset Example" width="400">
  <p><i>Example of superficial damage in a historical monument in Morelia.</i></p>
</div>

## ✨ Key Features
- **📸 High-Quality Imagery:** High-resolution images focused on capturing precise superficial damage on historical architecture.
- **🏛️ Real-World Scenarios:** Specifically targeted at temples and historical monuments in Morelia, capturing diverse textures, lighting, and degradation levels.
- **🧠 Ready for AI:** Fully annotated, preprocessed, and augmented to be directly used for training object detection and computer vision models (e.g., YOLO, ResNet).

## 📝 Dataset Description
This dataset is structured to facilitate the training and evaluation of machine learning models. The data distribution has been carefully divided to ensure optimal model performance:
- **75%** for Training 🏋️‍♂️
- **15%** for Validation 🔍
- **10%** for Testing 🧪

## 📊 Dataset Preprocessing & Augmentation
The dataset was carefully built using the following specifications to ensure robust model training and generalization:

- **Source Images:** 686
- **Classes:** 1 (Damage)
- **Data Split:** 75% Training / 15% Validation / 10% Testing

### Preprocessing
- **Auto-Orient:** Applied
- **Resize:** Stretch to 640x640

### Augmentation
- **Flip:** Horizontal, Vertical
- **90° Rotate:** Clockwise, Counter-Clockwise, Upside Down
- **Crop:** 0% Minimum Zoom, 20% Maximum Zoom
- **Rotation:** Between -9° and +9°
- **Saturation:** Between -25% and +25%
- **Noise:** Up to 0.1% of pixels

## 🛠️ Supported Frameworks

| 📦 Framework | 🚀 Usage |
| :--- | :--- |
| <img src="https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logo=YOLO&logoColor=black" alt="YOLO"> | **Object Detection:** This project is fully formatted, annotated, and **ready to be used directly in YOLO models** for training and inference. |
| <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"> | **Deep Learning Training:** Compatible with PyTorch-based computer vision pipelines and custom model architectures. |

## 📂 Project Architecture

```text
📦 Heritage_cracks/
├── 📁 CRACKS_PHONE.v2/           # Main dataset directory
│   ├── 📁 test/                  # Testing images and labels
│   └── 📁 train/                 # Training images and labels
│       ├── 📁 images/            # Augmented training images
│       └── 📁 labels/            # Bounding box labels
├── 📁 Images/                    # Repository images and assets
│   ├── 📄 EMAG.jpg               # Researcher photo
│   ├── 📄 JAGT1.jpg              # Researcher photo
│   └── 📄 Maybe.png              # Researcher photo
├── 📄 data.yaml                  # Dataset configuration file
├── 📄 README.dataset.txt         # Dataset documentation
├── 📄 README.roboflow.txt        # Roboflow export information
└── 📄 README.md                  # Project documentation (This file)
```

## 🧑‍🔬 Research Team

### 🌟 Meet the Team
Researchers advancing civil engineering, computer vision, and the preservation of historical heritage.

| Photo | Researcher | Affiliation | Contact |
| :---: | :--- | :--- | :---: |
| <img src="Images/Maybe.png" width="100" style="border-radius:50%;"> | **Maybeline Carolina García Chiquito** | | <a href="https://orcid.org/0009-0000-1793-4908"><img src="https://img.shields.io/badge/ORCID-0009--0000--1793--4908-a6ce39?logo=orcid&logoColor=white" alt="ORCID"></a> |
| <img src="Images/JAGT1.jpg" width="100" style="border-radius:50%;"> | **Dr. José Alberto Guzmán Torres** 🇲🇽 | SIIIA MATH | |
| <img src="Images/EMAG.jpg" width="100" style="border-radius:50%;"> | **Dra. Elia Mercedes Alonso Guzmán** 🇲🇽 | | |

## ⚖️ License
This dataset is released under the MIT License. You are free to use, modify, and distribute it, but please credit the authors appropriately.

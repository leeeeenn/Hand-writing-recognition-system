# Arabic Handwriting Recognition System

A deep learning-based handwriting recognition and writer identification system trained on the **AHAWP (Arabic Handwritten Automatic Word Processing)** dataset using CNN architectures, data augmentation, and transfer learning techniques.

The project explores multiple deep learning approaches for recognizing handwritten Arabic words and identifying anonymous users based on handwriting patterns.

Developed for the **Computer Vision (ENCS5343)** course at **Birzeit University**.

---

# Project Overview

This project investigates the effectiveness of different deep learning techniques for handwritten Arabic user identification.

The system was trained and evaluated through multiple stages:

1. Building and tuning a custom CNN architecture
2. Applying preprocessing and data augmentation techniques
3. Training a ResNet50 architecture
4. Applying transfer learning and fine-tuning on a pre-trained ResNet50 model

The final model achieved:

* **91.33% test accuracy**
* Improved generalization and stability
* Significant reduction in overfitting compared to earlier models

---

# Dataset

The project uses the **AHAWP dataset (Arabic Handwritten Automatic Word Processing)**.

Dataset characteristics:

* 82 different users/classes
* 10 Arabic words
* 10 handwriting samples per word
* Total of 8,144 handwritten images

Each image undergoes preprocessing before training.

---

# Features

* Custom CNN implementation from scratch
* Data preprocessing and image enhancement
* Data augmentation experiments
* Transfer learning using ResNet50
* Performance comparison between multiple architectures
* Accuracy/loss visualization and analysis
* GPU-accelerated deep learning experiments

---

# Technologies Used

* Python
* TensorFlow / Keras
* PyTorch
* OpenCV
* NumPy
* Matplotlib
* Scikit-learn
* PIL (Pillow)

---

# Preprocessing Pipeline

The preprocessing stage included:

* Grayscale conversion
* Image binarization
* Image inversion
* Reflection/mirroring
* Resizing
* Otsu thresholding

These preprocessing techniques significantly improved model accuracy and convergence.

---

# Model Evolution

## Task 1 — Custom CNN

* Built and optimized a custom CNN architecture
* Applied batch normalization and dropout
* Achieved approximately **50.49% accuracy**

## Task 2 — Data Augmentation

Applied augmentation techniques including:

* Rotation
* Width/height shifting
* Zooming
* Shearing

This improved test accuracy to approximately:

* **69.80%**

## Task 3 — ResNet50 Architecture

* Trained a ResNet50 model

* Compared against simpler architectures such as AlexNet

* Achieved:

* **83.24% test accuracy**

## Task 4 — Transfer Learning

* Fine-tuned a pre-trained ResNet50 model on ImageNet
* Combined feature extraction and fine-tuning strategies
* Added custom fully connected layers and dropout

Final performance:

* **91.33% test accuracy**

---

# Results Summary

| Model                        | Test Accuracy |
| ---------------------------- | ------------- |
| Custom CNN                   | 50.49%        |
| CNN + Data Augmentation      | 69.80%        |
| ResNet50                     | 83.24%        |
| Transfer Learning (ResNet50) | 91.33%        |

---

# Repository Structure

```text
Hand-writing-recognition-system
│
├── hand-recognition-system.ipynb     # Main notebook
├── reportproject.pdf                 # Full project report
├── README.md
└── .gitignore
```

---

# How to Run

1. Install dependencies:

```bash
pip install tensorflow torch torchvision matplotlib numpy scikit-learn pillow opencv-python
```

2. Open the notebook:

```bash
jupyter notebook hand-recognition-system.ipynb
```

3. Run the notebook cells sequentially.

---

# Concepts Demonstrated

This project demonstrates practical implementation of:

* Deep Learning
* CNN Architectures
* Transfer Learning
* Computer Vision
* Image Preprocessing
* Data Augmentation
* Model Evaluation and Optimization
* GPU-based Training

---

# Future Improvements

Potential future enhancements include:

* Vision Transformers (ViT)
* GAN-based dataset augmentation
* Real-time handwriting recognition deployment
* Arabic OCR system integration
* Larger-scale datasets and benchmarking

---

# Authors

* **Leen Ahmad**
* **Mai Zaid**

Computer Engineering Students
Birzeit University

# 😷 Face Mask Detection using CNN

A Deep Learning project for detecting whether a person is wearing a face mask or not using a Convolutional Neural Network (CNN).

## 📌 Project Overview

This project classifies face images into two categories:

- **With Mask**
- **Without Mask**

A CNN model is trained on labeled face images to learn visual patterns and predict mask usage.

---

## 🎯 Objective

The objective of this project is to:

- Build a CNN model for mask detection
- Perform image preprocessing and classification
- Learn deep learning workflow for computer vision tasks

---

## 📂 Dataset

Dataset used: **Face Mask Dataset**

Source: Kaggle  
Link: https://www.kaggle.com/datasets/omkargurav/face-mask-dataset

### Dataset Details
- **With Mask Images:** 3725
- **Without Mask Images:** 3828

**Total Images:** 7553

---

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- OpenCV
- Pillow (PIL)
- Scikit-learn
- Google Colab

---

## ⚙️ Workflow

### 1. Data Loading
- Downloaded dataset using Kaggle API
- Extracted dataset zip file

### 2. Image Preprocessing
- Loaded images from folders
- Resized images to **128 x 128**
- Converted images to RGB format
- Converted images into NumPy arrays

### 3. Label Encoding
- **With Mask → 1**
- **Without Mask → 0**

### 4. Data Splitting
- 80% Training Data
- 20% Testing Data

### 5. Data Normalization
- Scaled pixel values by dividing by 255

### 6. Model Building

CNN Architecture:

```python
Conv2D(32) + MaxPooling2D
Conv2D(64) + MaxPooling2D
Conv2D(128) + MaxPooling2D
Flatten
Dense(128) + Dropout
Dense(64) + Dropout
Output Layer
```

### 7. Model Training
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Epochs: 5

### 8. Model Evaluation
Model evaluated on test dataset.

---

## 📊 Results

### Accuracy
- **Training Accuracy:** 92.4%
- **Validation Accuracy:** 91.4%
- **Test Accuracy:** 93.25%

---

## 📈 Training Graphs

### Loss Graph
![Loss Graph](images/loss_graph.png)

### Accuracy Graph
![Accuracy Graph](images/accuracy_graph.png)

---

## 💾 Saved Model

Trained model saved as:

```bash
model.h5
```

---


---

## 🚀 Future Work

- Real-time webcam mask detection
- Web app deployment
- Transfer learning for improved accuracy

---

## 👨‍💻 Author

Aaditya Singh Tariyal

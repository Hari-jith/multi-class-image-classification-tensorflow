# 🐾 Multi-Class Image Classification using TensorFlow

A complete deep learning project demonstrating **multi-class image classification** using TensorFlow and Keras. This repository is designed for beginners and students learning computer vision and covers the entire workflow from building a Convolutional Neural Network (CNN) from scratch to applying Transfer Learning using MobileNetV2.

The project uses the **Animals-10** dataset from Kaggle and includes model evaluation, visualization, confusion matrix, prediction with confidence scores, and techniques to reduce overfitting.

---

## 📌 Features

- Build a CNN from scratch
- Train and evaluate a custom CNN
- Visualize training and validation performance
- Understand overfitting
- Apply Data Augmentation
- Use Early Stopping and ReduceLROnPlateau callbacks
- Implement Transfer Learning with MobileNetV2
- Generate Confusion Matrix
- Generate Classification Report
- Predict random images with confidence scores
- Beginner-friendly code with detailed comments and markdown explanations

---

## 📂 Dataset

Dataset used:

**Animals-10**

https://www.kaggle.com/datasets/alessiocorrado99/animals10

The dataset contains images belonging to the following classes:

- Dog
- Horse
- Elephant
- Butterfly
- Chicken
- Cat
- Cow
- Sheep
- Spider
- Squirrel

---

## 🧠 Models Implemented

### 1. Custom CNN

A Convolutional Neural Network built from scratch using:

- Conv2D
- MaxPooling2D
- Dense Layers
- Dropout
- ReLU Activation

This model demonstrates how CNNs learn image features from scratch and highlights the issue of overfitting.

---

### 2. Improved CNN

The custom CNN is enhanced using:

- Data Augmentation
- Dropout
- Early Stopping
- ReduceLROnPlateau

These techniques improve the model's ability to generalize to unseen data.

---

### 3. Transfer Learning (MobileNetV2)

A pretrained MobileNetV2 model is used as a feature extractor.

Advantages include:

- Faster training
- Higher validation accuracy
- Better generalization
- Reduced overfitting

---

## 📊 Evaluation Metrics

The project evaluates each model using:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss
- Confusion Matrix
- Classification Report
- Random Image Predictions
- Prediction Confidence Scores

---

## 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab / Kaggle Notebook

---

## 📁 Project Structure

```
├── notebooks/
│   └── image_classification.ipynb
│
├── Results/
│   ├── Custom_CNN/
│   ├── Improved_CNN/
│   └── MobileNet/
│   └── Strong_CNN/
│
├── README.md
└── requirements.txt
```

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/multi-class-image-classification-tensorflow.git
```

Move into the project directory

```bash
cd multi-class-image-classification-tensorflow
```

Install the required packages

```bash
pip install -r requirements.txt
```

---

## 📥 Download the Dataset

Using the Kaggle API

```python
import os

os.environ["KAGGLE_USERNAME"] = "YOUR_USERNAME"
os.environ["KAGGLE_KEY"] = "YOUR_API_KEY"

!kaggle datasets download -d alessiocorrado99/animals10
!unzip -q animals10.zip -d ./dataset
```

Dataset path:

```python
DATASET = "/content/dataset/raw-img"
```

---

## 📈 Sample Results

The project demonstrates:

- CNN from scratch
- Improved CNN using regularization techniques
- MobileNetV2 Transfer Learning

Example outputs include:

- Accuracy/Loss Curves
- Confusion Matrix
- Classification Report
- Random Image Predictions with Confidence Scores

---

## 🎯 Learning Outcomes

By completing this project, you will understand:

- Image preprocessing
- Multi-class image classification
- Building CNNs from scratch
- Overfitting and regularization
- Data Augmentation
- Callbacks in TensorFlow
- Transfer Learning
- Model evaluation techniques
- Prediction and confidence estimation

---

## 📚 Requirements

- Python 3.10+
- TensorFlow
- NumPy
- Matplotlib
- Scikit-learn

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## ⭐ Acknowledgements

- TensorFlow
- Keras
- Kaggle
- Animals-10 Dataset by Alessio Corrado

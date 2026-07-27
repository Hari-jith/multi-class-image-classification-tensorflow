# 🐾 Multi-Class Image Classification using TensorFlow

A comprehensive deep learning project demonstrating **multi-class image classification** using TensorFlow and Keras. This repository covers the complete workflow of building image classification models—from a **Convolutional Neural Network (CNN) from scratch** to **Transfer Learning using MobileNetV2**—using the **Animals-10** dataset.

The project is designed for **students, beginners, and educators** to understand CNNs, overfitting, regularization techniques, data augmentation, callbacks, transfer learning, and model evaluation.

---

# 📌 Project Objectives

- Build a CNN from scratch for multi-class image classification.
- Analyze overfitting using training and validation curves.
- Improve model generalization using Data Augmentation and Callbacks.
- Compare custom CNNs with a pretrained MobileNetV2 model.
- Evaluate models using Confusion Matrix and Classification Report.
- Predict random validation images with confidence scores.

---

# 📂 Dataset

**Dataset:** Animals-10

**Source:** https://www.kaggle.com/datasets/alessiocorrado99/animals10

The dataset contains approximately **28,000+ images** across **10 animal classes**.

### Classes

- 🐶 Dog
- 🐴 Horse
- 🐘 Elephant
- 🦋 Butterfly
- 🐔 Chicken
- 🐱 Cat
- 🐄 Cow
- 🐑 Sheep
- 🕷 Spider
- 🐿 Squirrel

---

# 🧠 Models Implemented

## 1. Custom CNN

A CNN built completely from scratch using:

- Convolution Layers
- MaxPooling
- Dense Layers
- Dropout

This model demonstrates how CNNs learn features directly from the dataset and highlights the problem of **overfitting**.

---

## 2. Improved CNN

The custom CNN is improved by incorporating:

- Data Augmentation
- Early Stopping
- ReduceLROnPlateau
- Dropout Regularization

The goal is to improve generalization and reduce overfitting.

---

## 3. MobileNetV2 (Transfer Learning)

A pretrained MobileNetV2 model is used as a feature extractor.

Advantages include:

- Faster convergence
- Better feature extraction
- Higher validation accuracy
- Reduced overfitting
- Excellent generalization

---

## 4. Strong CNN

A deeper CNN architecture consisting of:

- Multiple Convolution Blocks
- Batch Normalization
- Global Average Pooling
- Dropout
- Dense Layers

This model was implemented to explore whether a deeper CNN trained from scratch could outperform a pretrained model.

---

# 📊 Model Performance

| Model | Training Accuracy | Validation Accuracy | Validation Loss | Observation |
|--------|------------------:|--------------------:|----------------:|-------------|
| **Custom CNN** | **93.16%** | **66.61%** | **1.7305** | Severe Overfitting |
| **Improved CNN** | **70.12%** | **66.30%** | **1.0008** | Better Generalization |
| **Strong CNN** | **70.79%** | **63.72%** | **1.1208** | Underperformed on this dataset |
| **MobileNetV2** | **83.28%** | **91.86%** | **0.2608** | Best Overall Performance |

---

# 📈 Key Observations

### Custom CNN

- Achieved high training accuracy.
- Large gap between training and validation accuracy.
- Clearly demonstrates **overfitting**.

---

### Improved CNN

- Reduced overfitting using Data Augmentation and Callbacks.
- Validation loss improved significantly.
- More stable training compared to the baseline CNN.

---

### Strong CNN

Although architecturally deeper, the Strong CNN did not outperform the simpler models. This demonstrates that **a more complex architecture does not necessarily guarantee better performance**, especially when training from scratch on a limited dataset.

---

### MobileNetV2

The pretrained MobileNetV2 model achieved the highest validation accuracy and lowest validation loss. This highlights the effectiveness of **Transfer Learning**, where previously learned visual features from ImageNet are reused for a new classification task.

---

# 📊 Evaluation Metrics

Each model is evaluated using:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss
- Confusion Matrix
- Classification Report
- Random Image Prediction
- Prediction Confidence Score

---

# 📁 Project Structure

```text
├── multi_class_classification_cnn.ipynb
│
├── Results/
│   ├── Custom_CNN/
│   ├── Improved_CNN/
│   ├── MobileNet/
│   └── Strong_CNN/
│
├── README.md
└── requirements.txt
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/Hari-jith/multi-class-image-classification-tensorflow.git
```

Navigate to the project directory

```bash
cd multi-class-image-classification-tensorflow
```

Install the dependencies

```bash
pip install -r requirements.txt
```

---

# 📥 Download the Dataset

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

# 📈 Results

The repository includes the outputs generated for every model, including:

- Training & Validation Accuracy Curves
- Training & Validation Loss Curves
- Confusion Matrix
- Classification Report
- Random Predictions with Confidence Scores

The result images are organized under the **Results** directory for easy comparison.

---

# 🎯 Learning Outcomes

This project helps learners understand:

- Image preprocessing
- Multi-class image classification
- CNN architecture
- Feature extraction using convolution
- Overfitting
- Data Augmentation
- Early Stopping
- Learning Rate Scheduling
- Transfer Learning
- Model Evaluation
- Prediction with Confidence Scores

---

# 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab
- Kaggle

---

# 📦 Requirements

- Python 3.10+
- TensorFlow
- NumPy
- Matplotlib
- Scikit-learn

Install using:

```bash
pip install -r requirements.txt
```

---

# 🙏 Acknowledgements

- TensorFlow & Keras
- Kaggle
- Animals-10 Dataset by Alessio Corrado
- Google Colab

---

# 📜 License

This project is released for **educational and learning purposes**.

Feel free to fork the repository, modify the code, and use it for academic or personal learning projects.

---

## ⭐ If you found this project useful, consider giving the repository a star!

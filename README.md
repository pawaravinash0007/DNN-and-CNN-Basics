<div align="center">

# 🧠 DNN-and-CNN-Basics

### Deep Learning Fundamentals — DNN & CNN with Fashion MNIST

[![Language](https://img.shields.io/badge/Language-Python-blue?style=flat-square&logo=python)](.)
[![Framework](https://img.shields.io/badge/Framework-TensorFlow%20%7C%20Keras-FF6F00?style=flat-square&logo=tensorflow)](.)
[![Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange?style=flat-square&logo=jupyter)](.)
[![Dataset](https://img.shields.io/badge/Dataset-Fashion%20MNIST-purple?style=flat-square)](.)

</div>

---

## 📖 Overview

A hands-on introduction to **Deep Neural Networks (DNN)** and **Convolutional Neural Networks (CNN)** using the **Fashion MNIST** dataset. This project walks through building, training, and evaluating neural networks from scratch using TensorFlow/Keras, with clear explanations of each layer and concept.

---

## 🎯 Learning Objectives

- Understand the architecture of Dense (fully connected) neural networks
- Build and train a CNN for image classification
- Compare DNN vs CNN performance on image data
- Visualize training curves, confusion matrices, and feature maps
- Apply regularization techniques (Dropout, Batch Normalization)

---

## 📊 Dataset — Fashion MNIST

| Property | Details |
|----------|---------|
| **Classes** | 10 (T-shirt, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot) |
| **Training samples** | 60,000 grayscale images |
| **Test samples** | 10,000 grayscale images |
| **Image size** | 28×28 pixels |

---

## 🏗️ Model Architectures

### DNN (Dense Neural Network)
```
Input (784) → Dense(256, ReLU) → Dropout(0.3)
           → Dense(128, ReLU) → Dropout(0.3)
           → Dense(10, Softmax)
```

### CNN (Convolutional Neural Network)
```
Input (28×28×1) → Conv2D(32, 3×3, ReLU) → MaxPool(2×2)
               → Conv2D(64, 3×3, ReLU) → MaxPool(2×2)
               → Flatten → Dense(128, ReLU) → Dropout(0.5)
               → Dense(10, Softmax)
```

---

## 📈 Results

| Model | Test Accuracy | Parameters |
|-------|-------------|-----------|
| DNN | ~88% | ~270K |
| CNN | ~92% | ~420K |

> CNN outperforms DNN by ~4% on image classification tasks.

---

## 🚀 Getting Started

```bash
git clone https://github.com/pawaravinash0007/DNN-and-CNN-Basics.git
cd DNN-and-CNN-Basics
pip install tensorflow numpy matplotlib seaborn jupyter
jupyter notebook DNN_CNN_FashionMNIST.ipynb
```

---

## 📁 Repository Structure

```
DNN-and-CNN-Basics/
├── DNN_FashionMNIST.ipynb      # Dense network notebook
├── CNN_FashionMNIST.ipynb      # Convolutional network notebook
├── utils/
│   └── visualization.py        # Plotting utilities
└── README.md
```

---

## 🛠️ Tech Stack

`Python` · `TensorFlow` · `Keras` · `NumPy` · `Matplotlib` · `Seaborn` · `Jupyter`

---

## 👤 Author

**Avinash Pawar** | [@pawaravinash0007](https://github.com/pawaravinash0007)

<div align="center">⭐ Star this repo if you find it useful! ⭐</div>

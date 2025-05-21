# 🧠 MNIST Digit Classifier (PyTorch)

This project implements a **Convolutional Neural Network (CNN)** in **PyTorch** to classify handwritten digits (0–9) from the **MNIST** dataset.  
Compared to a simple feedforward model, this version achieves **higher accuracy** by leveraging CNN layers and **Dropout** to reduce overfitting.

## ✅ Features
- 🔍 **CNN-based model** for improved accuracy on image data
- 🧹 **Dropout layers** to prevent overfitting
- 📉 **Loss visualization** over training epochs
- 📊 **Confusion matrix** for error analysis
- 💾 Saves trained model as `.pth`
- ☁️ Fully **Google Colab** compatible
- 🧪 Achieves ~**99% test accuracy**

## 🏃‍♂️ Run it on Colab
![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)
(https://github.com/Gorachand2501/mnist-digit-classifier/blob/main/MNIST_Digit_Calssification%20(CNN).ipynb)

## 📦 Requirements
- torch
- torchvision
- matplotlib
- scikit-learn

## 🧠 Model Architecture
Input: 28x28 grayscale image  
Conv2D(1, 32, 3x3) → ReLU  
Conv2D(32, 64, 3x3) → ReLU  
→ MaxPooling(2x2) → Dropout(0.25)  
→ Flatten  
→ Linear(9216 → 128) → ReLU → Dropout(0.5)  
→ Linear(128 → 10)

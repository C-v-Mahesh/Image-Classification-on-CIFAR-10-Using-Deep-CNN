# 📸 Image Classification on CIFAR-10 Using Deep Convolutional Neural Networks

This repository contains the implementation of a Deep Convolutional Neural Network (CNN) built from scratch to classify images from the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html). The project demonstrates how deep learning outperforms traditional machine learning models on complex image classification tasks.

---

## 🧠 Project Overview

- Dataset: **CIFAR-10**
- Image Size: **32×32 RGB images**
- Classes: `Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck`
- Model Type: **Custom Deep CNN**
- Goal: Achieve high classification accuracy using CNN, data augmentation, and regularization.

---

## 🛠️ Key Features

- Custom CNN model using `TensorFlow` and `Keras`
- Data preprocessing and normalization
- Real-time **data augmentation** (rotation, flipping, shifting)
- **Early stopping** to prevent overfitting
- **Performance visualization** (accuracy, loss, confusion matrix)
- **Comparison with traditional models** like SVM, KNN, and HOG

---

## 🧩 Model Architecture

| Layer                  | Type                     | Output Shape | Parameters |
|-----------------------|--------------------------|--------------|------------|
| Conv2D                | ReLU, 32 filters          | 32×32×32     | 896        |
| MaxPool2D             | 2×2                       | 16×16×32     | 0          |
| Conv2D                | ReLU, 64 filters          | 16×16×64     | 18,496     |
| MaxPool2D             | 2×2                       | 8×8×64       | 0          |
| Conv2D                | ReLU, 128 filters         | 8×8×128      | 73,856     |
| MaxPool2D             | 2×2                       | 4×4×128      | 0          |
| Conv2D                | ReLU, 256 filters         | 4×4×256      | 295,168    |
| GlobalAveragePooling2D|                          | 256          | 0          |
| Dense                 | ReLU, 128 units           | 128          | 32,896     |
| Dropout               | Rate = 0.5                | 128          | 0          |
| Dense                 | Softmax (10 classes)      | 10           | 1,290      |

**Total Parameters:** 422,602

---

## 📊 Results

| Model            | Accuracy (%) | Test Loss (%) |
|------------------|--------------|----------------|
| SVM (Linear)     | 36           | 44             |
| SVM (Polynomial) | 40           | 42             |
| HOG              | 40           | 50             |
| KNN              | 34           | 66             |
| **CNN (This Work)** | **74.7**     | **26**         |

> 📌 Paper model accuracy (after tuning): **88%**

---

## 📁 File Structure


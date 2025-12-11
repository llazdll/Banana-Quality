# 🍌 Banana Quality Classification using PyTorch

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-yellow.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

A binary classification project that predicts **banana quality** as **Good (1)** or **Bad (0)** using a simple neural network built with **PyTorch**. This project uses a dataset from Kaggle and demonstrates a full machine-learning workflow: preprocessing, training, validation, evaluation, and visualization.

---

## 📂 Dataset

Loaded from:
https://www.kaggle.com/datasets/l3llff/banana

### Features
- Size  
- Weight  
- Sweetness  
- Softness  
- HarvestTime  
- Ripeness  
- Acidity  

### Target
- **Quality:**  
  - Good → 1  
  - Bad → 0  

---

## 🧹 Data Preprocessing

- Load the CSV file using pandas  
- Encode labels (`Good = 1`, `Bad = 0`)  
- Split into training, validation, and test sets  
- Normalize all input features using `StandardScaler`  
- Convert NumPy arrays to PyTorch tensors  
- Build DataLoaders for efficient batching  

---

## 🧠 Model Overview

A simple logistic regression model:

nn.Sequential(
nn.Linear(7, 1),
nn.Sigmoid()
)

**Loss Function:** Binary Cross Entropy (BCELoss)  
**Optimizer:** SGD with lr=0.1 and momentum=0.9  
**Epochs:** 10  

---

## 🚀 Training

The script performs:

- Forward propagation  
- BCE loss computation  
- Backpropagation  
- Weight updates using SGD  
- Validation at each epoch  
- Tracking:  
  - Training & Validation Loss  
  - Training & Validation Accuracy  

Example training output:

Epoch: 0 LossTrain: 0.35 AccTrain: 0.83 LossValid: 0.28 AccValid: 0.88
...
Epoch: 9 LossTrain: 0.29 AccTrain: 0.88 LossValid: 0.28 AccValid: 0.88

3. Click **Run All**  

---

## 📦 Requirements

numpy
pandas
matplotlib
scikit-learn
torch

---

## 📜 Project Goals

This project demonstrates:

- Binary classification using PyTorch  
- Data normalization and preprocessing  
- Custom training loop  
- Model evaluation  
- Metric visualization  

---

## 🤝 Contributing

Contributions and suggestions are welcome.  
Feel free to open issues or submit pull requests.

---

## ⭐ Support

If this project was helpful, please **star the repository**!

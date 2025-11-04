# Neural Network for Network Intrusion Detection (UNSW-NB15 Dataset)

This project implements a **Multi-Layer Perceptron (MLP)** from scratch using **NumPy** to classify network traffic as normal or attack based on the **UNSW-NB15** dataset.  
It demonstrates core machine learning concepts - data preprocessing, feature engineering, model building, training, and performance evaluation, without relying on deep learning frameworks like TensorFlow or PyTorch.

---

## 🧠 Project Overview

- **Goal:** Detect network intrusions using a neural network model built entirely from first principles.
- **Dataset:** [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset) (training, testing1, testing2 subsets)
- **Approach:** Custom implementation of an MLP (feedforward neural network) with:
  - ReLU and Sigmoid activations
  - He initialization for stable training
  - Binary Cross-Entropy loss
  - Batch Gradient Descent optimization

---

## ⚙️ Steps in the Notebook

1. **Data Loading:**  
   Load and inspect training and test CSV files.

2. **Data Preprocessing:**  
   - One-hot encode categorical variables (`proto`, `service`, `state`)  
   - Align train/test columns  
   - Standardize features using Z-score normalization  

3. **Model Implementation:**  
   - Implement forward and backward propagation manually  
   - Define activation, derivative, and loss functions  
   - Train with epochs and learning rate tuning

4. **Evaluation Metrics:**  
   - Confusion Matrix  
   - Accuracy, Balanced Accuracy  
   - Precision, Recall, F1-score  

---

## 📊 Results

| Metric | Value |
|---------|-------|
| **Accuracy (Test Set 1)** | 0.905 |
| **Balanced Accuracy** | 0.917 |
| **Precision** | 0.975 |
| **Recall** | 0.882 |
| **F1-score** | 0.926 |

The model shows strong generalization with balanced performance between precision and recall.

---

## 🧩 Predicted Labels for Test Set 2

Example predictions for 25 samples (0 = normal, 1 = attack):


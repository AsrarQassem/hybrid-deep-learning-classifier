# hybrid-deep-learning-classifier

> A multi-model deep learning system combining CNN, MLP, and RNN architectures for robust image classification.

---

## 📌 Overview

This project implements a **hybrid deep learning approach** by combining three different neural network architectures:

* Convolutional Neural Network (CNN)
* Multilayer Perceptron (MLP)
* Recurrent Neural Network (RNN / LSTM)

Each model learns different patterns from the data, and their predictions are combined to improve overall performance.

---

## 🏗️ Models Architecture

### 🔹 CNN (Convolutional Neural Network)

* Extracts spatial features from images
* Uses convolution + pooling layers
* Strong performance on image classification

### 🔹 MLP (Multilayer Perceptron)

* Fully connected network
* Works on flattened image data
* Learns global relationships

### 🔹 RNN / LSTM

* Treats images as sequences
* Captures row-wise dependencies
* Provides a unique perspective compared to CNN

---

## 🔗 Hybrid Strategy (Soft Voting)

Each model outputs a probability distribution over classes.

👉 Final prediction is computed by:

* Averaging probabilities from all models
* Selecting the class with highest average score

✔ This approach improves:

* Accuracy
* Stability
* Generalization

---

## 📊 Results

| Model            | F1 Score   | Precision  | Recall     | Accuracy   |
| ---------------- | ---------- | ---------- | ---------- | ---------- |
| CNN              | 0.9036     | 0.9040     | 0.9036     | 0.9036     |
| MLP              | 0.8881     | 0.8890     | 0.8891     | 0.8891     |
| RNN (LSTM)       | 0.9002     | 0.9007     | 0.9011     | 0.9011     |
| **Hybrid Model** | **0.9203** | **0.9205** | **0.9208** | **0.9208** |

🚀 The hybrid model outperforms all individual models.

---

## 🧪 Training Details

* Optimizer: Adam
* Loss Function: Categorical Crossentropy
* Epochs: 10
* Validation Split: 20%

---
## License

<span style="font-size:0.9em; white-space:nowrap;">
  <a href="https://github.com/AsrarQassem/hybrid-deep-learning-classifier">hybrid-deep-learning-classifier</a> © 2024 by 
  <a href="https://github.com/AsrarQassem">Asrar Qassem</a> · 
  <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0</a>

  <img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" style="width:14px;height:14px;vertical-align:-2px;margin-left:4px;">
  <img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" style="width:14px;height:14px;vertical-align:-2px;">
  <img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" style="width:14px;height:14px;vertical-align:-2px;">
  <img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" style="width:14px;height:14px;vertical-align:-2px;">
</span>

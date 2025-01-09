# Neural Network for Digit Recognition

This repository contains an implementation of a neural network for recognizing handwritten digits, inspired by the famous MNIST dataset. The project demonstrates building, training, and testing a neural network using Python and relevant libraries.


## Project Overview

The goal of this project is to classify images of handwritten digits (0-9) using a neural network. The dataset consists of grayscale images represented as numerical arrays. The model is trained to accurately predict the digit represented by each image.

---

## Dataset

### Files:
- `train_X.csv`: Training data features (input images as flattened arrays).
- `train_label.csv`: Training data labels (corresponding digit labels).
- `test_X.csv`: Test data features for evaluation.
- `test_label.csv`: Test data labels for accuracy calculation.

### Description:
- **Input features:** Grayscale pixel values ranging from 0 to 255 (28x28 images, flattened to a 784-length vector).
- **Labels:** Integer values from 0 to 9 representing the digit.

---

## How It Works

1. **Preprocessing:**
   - Normalize pixel values to a range of 0 to 1.
   - Split the dataset into training and testing sets.

2. **Neural Network:**
   - Input layer: 784 nodes (one for each pixel).
   - Hidden layers: Configurable, with activation functions (e.g., ReLU).
   - Output layer: 10 nodes (one for each digit), using softmax activation.

3. **Training:**
   - Loss function: Cross-entropy.
   - Optimizer: Stochastic Gradient Descent (SGD) or Adam.
   - Metrics: Accuracy.

4. **Evaluation:**
   - Test the model on unseen data using `test_X.csv` and compare predictions with `test_label.csv`.


# MNIST Handwritten Digit Classification

> Comparing a simple Neural Network and Logistic Regression for handwritten digit classification using the MNIST dataset.

## Overview

This project explores two machine learning approaches for classifying handwritten digits from the **MNIST dataset**:

1. A simple **Neural Network**
2. A **Logistic Regression** model

Both models are trained and evaluated using the same MNIST data, providing a practical comparison between a traditional machine learning classification algorithm and a basic neural network.

The project was developed to understand the fundamentals of image classification, model training, and the differences between classical machine learning and neural networks.

## The Problem

The MNIST dataset contains grayscale images of handwritten digits ranging from **0 to 9**.

The goal is to build models that can correctly identify which digit is represented by a given image.

```text
Input:  28 × 28 handwritten digit image
                ↓
             Model
                ↓
Output: Predicted digit (0–9)
```

## Dataset

MNIST contains **70,000 handwritten digit images**, with each image having a resolution of **28 × 28 pixels**.

Each image represents one of ten classes:

```text
0  1  2  3  4  5  6  7  8  9
```

The image data is represented as numerical pixel values and prepared for use by both models.

## Models

### 1. Neural Network

A simple feedforward neural network is used to classify the handwritten digits.

The image pixels are provided as input to the network, which learns patterns associated with each digit and produces a prediction across the ten digit classes.

The model achieved:

**Test Accuracy: 97.90%**

The reported evaluation result was:

```text
Loss:     0.0760
Accuracy: 0.9790
```

### 2. Logistic Regression

A Logistic Regression classifier is also trained on the same MNIST data.

Because Logistic Regression expects tabular feature vectors, each 28 × 28 image is flattened into a **784-dimensional vector** before being provided to the model.

The model achieved:

**Test Accuracy: 92.00%**

## Model Comparison

| Model               | Input Representation       | Accuracy |
| ------------------- | -------------------------- | -------: |
| Logistic Regression | Flattened 784-pixel vector |   92.00% |
| Neural Network      | 784-pixel input            |   97.90% |

The Neural Network achieved a higher classification accuracy than Logistic Regression on the same task.

The difference demonstrates how a neural network can learn more complex non-linear relationships in image data than a basic linear classification model.

## Machine Learning Workflow

```text
MNIST Dataset
      ↓
Data Preparation
      ↓
Image Preprocessing
      ↓
Train/Test Split
      ↓
 ┌───────────────┐
 │               │
 ↓               ↓
Logistic       Neural
Regression     Network
 │               │
 ↓               ↓
Predictions    Predictions
 │               │
 └───────┬───────┘
         ↓
   Model Evaluation
         ↓
   Accuracy Comparison
```

## Concepts Practiced

This project helped me practice:

* Image classification
* Working with the MNIST dataset
* Image preprocessing
* Flattening image data
* Multi-class classification
* Logistic Regression
* Neural Networks
* Model training and evaluation
* Comparing machine learning approaches
* Interpreting classification accuracy

## Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Scikit-learn**
* **TensorFlow / Keras**
* **Matplotlib** (if used for visualization)

## Project Structure

```text
mnist-classification/
│
├── neural_network/
│   └── ...
│
├── logistic_regression/
│   └── ...
│
├── dataset/
│   └── ...
│
└── README.md
```

## Results

The two models produced different levels of performance:

* **Neural Network:** 97.90%
* **Logistic Regression:** 92.00%

The Neural Network outperformed Logistic Regression by approximately **5.9 percentage points**.

This comparison provided a practical demonstration of the advantages of neural networks for image classification tasks.

## Project Status

**Completed**

This project serves as an introduction to neural networks and provides a direct comparison between a traditional machine learning classifier and a neural-network-based approach on the same image classification problem.

## Future Improvements

Potential improvements include:

* Experimenting with different neural network architectures
* Adding hidden layers and neurons
* Applying regularization
* Tuning model hyperparameters
* Visualizing incorrect predictions
* Building a Convolutional Neural Network (CNN)
* Comparing additional classification algorithms

## Author

**Ruvarashe Nemaramba**

Artificial Intelligence Student & Developer

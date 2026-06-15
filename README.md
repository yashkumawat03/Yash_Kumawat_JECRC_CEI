# Week 4 Assignment: CIFAR-10 Image Classification using ANN and CNN

## Overview

This project focuses on image classification using the CIFAR-10 dataset. The objective is to compare the performance of Artificial Neural Networks (ANNs) and Convolutional Neural Networks (CNNs) on a multi-class image classification task and analyze the impact of different training strategies.

---

## Dataset

The CIFAR-10 dataset contains:

- 50,000 training images
- 10,000 test images
- 10 classes:
  - Airplane
  - Automobile
  - Bird
  - Cat
  - Deer
  - Dog
  - Frog
  - Horse
  - Ship
  - Truck

Image size: **32 × 32 × 3 (RGB)**

---

## Project Workflow

### 1. Data Loading and Preprocessing
- Loaded CIFAR-10 dataset from TensorFlow/Keras.
- Visualized sample images from each class.
- Normalized pixel values from 0–255 to 0–1 for stable training.

### 2. Baseline ANN Model
- Flatten layer
- Dense layers with ReLU activation
- Dropout regularization
- Softmax output layer

### 3. Baseline CNN Model
- Conv2D layers
- Batch Normalization
- Max Pooling
- Dense classification layer
- Softmax output layer

### 4. Model Training
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Epochs: 10
- Validation Split: 20%

### 5. Performance Comparison
- Compared validation accuracy curves of ANN and CNN.
- Evaluated test accuracy of both models.

---

## Advanced Experiments

### Deep ANN
- Increased the number of Dense layers.
- Analyzed performance improvement over the baseline ANN.

### Enhanced CNN
- Increased filter sizes:
  - 32
  - 64
  - 128
- Improved feature extraction capability.

### Extended Training
- Increased training duration from 10 to 20 epochs.
- Observed model learning behavior.

### EarlyStopping
- Implemented EarlyStopping callback.
- Prevented overfitting and restored best model weights.

### Data Augmentation
Applied:
- RandomFlip
- RandomRotation
- RandomZoom

Improved model generalization on unseen data.

---

## Results

| Model | Accuracy |
|--------|----------|
| ANN | 38.91% |
| CNN | 67.68% |

CNN significantly outperformed ANN by preserving spatial information and learning hierarchical image features through convolution operations.

---

## Key Learnings

- CNNs are better suited for image classification than ANNs.
- Increasing network depth can improve learning capacity.
- Larger convolutional filter stacks improve feature extraction.
- Data augmentation improves generalization.
- EarlyStopping helps reduce overfitting and unnecessary training.

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib

---

## Conclusion

This assignment demonstrated the effectiveness of Convolutional Neural Networks for image classification tasks. Through multiple experiments involving architecture changes, training strategies, and data augmentation, the project highlighted how different design choices impact model performance and generalization ability on the CIFAR-10 dataset.

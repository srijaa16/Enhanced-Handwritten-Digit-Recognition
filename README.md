Enhanced Handwritten Digit Recognition Using ANN with RBM-Based Features

An enhanced handwritten digit recognition system using an Artificial Neural Network (ANN) with Restricted Boltzmann Machine (RBM)-based feature extraction.

Project Overview

This project focuses on recognizing handwritten digits from the MNIST dataset using an ANN model.

A baseline ANN model using the original 784 pixel features is compared with ANN models trained on features extracted using RBM.

The project evaluates different RBM feature sizes to study their effect on classification performance.

Dataset

- Dataset: MNIST Handwritten Digits
- Training Images: 60,000
- Testing Images: 10,000
- Image Size: 28 × 28 pixels
- Classes: 10 (digits 0–9)
- Pixel values are normalized between 0 and 1.

Methodology

1. Data Preprocessing
   - Normalize pixel values
   - Flatten 28 × 28 images into 784 features

2. Baseline ANN
   - An ANN is trained directly using the original 784 features.

3. RBM Feature Extraction
   - RBM is used to transform the original 784-dimensional representation into lower-dimensional feature representations.
   - Experiments were conducted using 128, 256, and 384 RBM features.

4. ANN Classification
   - The extracted RBM features are given as input to an ANN classifier for digit recognition.

Results

| Model | Features | Test Accuracy |
|---|---:|---:|
| Baseline ANN | 784 | 97.80% |
| RBM + ANN | 128 | 95.60% |
| RBM + ANN | 256 | 97.61% |
| RBM + ANN | 384 | 97.64% |

The 384-feature RBM + ANN model achieved 97.64% test accuracy while reducing the feature representation from 784 to 384 features.

Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- MNIST Dataset
- Restricted Boltzmann Machine (RBM)
- Artificial Neural Network (ANN)

Project File

- Enhanced_Handwritten_Digit_Recognition.ipynb – Complete implementation, experiments, evaluation and results.

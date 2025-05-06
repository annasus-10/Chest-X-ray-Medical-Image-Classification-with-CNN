# Chest X-ray Medical Image Classification with CNN

## Overview
This project involves classifying Chest X-ray images as either normal or pneumonia using a Convolutional Neural Network (CNN) in TensorFlow and Keras. The model is built to accurately perform binary classification on grayscale medical images.

## Dataset
- **Dataset Source:** [Chest X-Ray Images (Pneumonia) on Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- **Structure:** The dataset contains three folders: `train`, `val`, and `test`, each with subfolders for "NORMAL" and "PNEUMONIA" images.
- **Images:** Grayscale, anterior-posterior chest X-rays

## Data Preparation
- **Image Resizing:** All images resized to 128x128 pixels
- **Color Mode:** Grayscale
- **Batch Size:** 32
- **Data Augmentation:** Applied using `ImageDataGenerator` for increased robustness
- **Splits:** Supplied train/val/test folders used for training, validation, and testing

## Model Architecture
- **Base Model:** Convolutional Neural Network (CNN)
- **Input:** 128x128 grayscale images
- **Layers:**  
  - Multiple convolutional and pooling layers for feature extraction
  - Dropout layers for regularization
  - Dense layers for classification
- **Output:** Single neuron with sigmoid activation for binary classification

## Training Details
- **Loss Function:** Binary cross-entropy
- **Optimizer:** Adam
- **Accuracy Target:** Trained to achieve at least 90% accuracy on test data

## Evaluation
- **Test Accuracy:** Achieved test accuracy of 96%

## References
- [Chest X-Ray Images (Pneumonia) Dataset on Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- TensorFlow & Keras documentation

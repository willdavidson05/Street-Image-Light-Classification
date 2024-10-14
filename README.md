# Street Light Image Classification using SVM and CNN

## Overview

This project aims to classify street light images into three categories: **Red**, **Yellow**, and **Green** using two machine learning models: **Support Vector Machines (SVMs)** and **Convolutional Neural Networks (CNNs)**. The project explores the effectiveness of both models, comparing their performance in classifying images of street lights.

## Models

### Support Vector Machine (SVM)

The **SVM model** was trained on the street light dataset to classify images into **Red**, **Yellow**, or **Green** categories. SVMs are well-suited for small to medium-sized datasets, and the model performed effectively on this task. It served as a baseline model for comparison with more complex architectures like CNN.

- **Kernel**: The SVM used a radial basis function (RBF) kernel to classify the images.
- **Performance**: The SVM model achieved competitive results, particularly in classifying **Red** lights with zero misclassifications.

### Convolutional Neural Network (CNN)

A **CNN** was implemented to handle the more complex nuances of image data. CNNs are highly effective for image classification tasks, as they can automatically learn spatial hierarchies in images. 

Key features of the CNN include:

- **Architecture**: Multiple convolutional layers, pooling layers, and fully connected layers.
- **Activation functions**: ReLU for non-linearity and softmax for output classification.
- **Optimizer**: Adam optimizer for efficient weight updates.
- **Loss function**: Categorical crossentropy.

The CNN was trained for **X epochs**, achieving an accuracy of **99.58%** on the test set, slightly outperforming the SVM.

## Evaluation

Both models were evaluated using the following metrics:

- **Accuracy**: 
  - SVM: High accuracy with strong performance, particularly in the **Red** light classification.
  - CNN: Achieved 99.58% accuracy with fewer misclassifications, especially in **Yellow** light classifications.
  
- **Confusion Matrix**:
  - SVM: Minimal misclassifications.
  - CNN: Zero errors for **Red** lights, and very few errors for **Yellow** and **Green**.

- **Loss/Accuracy Graphs (CNN)**: The CNN demonstrated stable training with minor divergence in the early epochs, which quickly stabilized.
# Image Binary Classification Project

## Overview

This project focuses on the binary classification of automobile and motorcycle images using three different machine learning methods: Naïve Bayes, k-Nearest Neighbors (k-NN), and Artificial Neural Networks (ANN). The goal is to compare the performance of these models in terms of accuracy, computational efficiency, and other relevant metrics.

## Project Structure

The project contains the following files:

- `ANN.py`: Code for the Artificial Neural Network model.
- `KNN.py`: Code for the k-Nearest Neighbors model.
- `Naive_bayes_classifier.py`: Code for the Naïve Bayes Classifier model.
- `FinalReport.pdf`: The final report detailing the project, including methodology, results, and conclusions.

## Dataset

The dataset consists of car and motorcycle images from different sources:
- Car images are from a Kaggle dataset.
- Motorcycle images are from Image-CV.

The dataset is preprocessed to ensure uniform image sizes and is divided into training and testing sets. Images are labeled as 0 (car) and 1 (motorcycle).

## Preprocessing

For Naïve Bayes and k-NN, preprocessing includes:
- Resizing images to a uniform size.
- Converting images to grayscale.
- Extracting color histograms.
- Normalizing features.
- Applying Principal Component Analysis (PCA) for dimensionality reduction.

For ANN, preprocessing includes:
- Resizing images.
- Converting images to grayscale.
- Normalizing pixel values.

## Methods

### 1. Naïve Bayes Classifier

Implemented using Gaussian Naïve Bayes, this classifier assumes that features are conditionally independent. It performs classification based on the likelihood of features given the class.

- **Accuracy**: Achieved an accuracy of 0.64 with 20 PCA components.

### 2. k-Nearest Neighbors (k-NN)

This non-parametric method classifies data points based on the majority class of their k-nearest neighbors in the feature space.

- **Best k-value**: Found to be 22.
- **Accuracy**: Achieved a maximum accuracy of 0.788.

### 3. Artificial Neural Network (ANN)

A custom neural network implementation without using any ML libraries. It includes two hidden layers with ReLU activation and a dropout layer to prevent overfitting.

- **Accuracy**: Achieved an accuracy of 0.889.

## Cross-Validation
The project uses k-fold cross-validation to validate the models' performance. The results are compared with the test set results to ensure consistency and robustness.

## Results
The ANN model outperformed the other methods in terms of accuracy and robustness. The results from the project indicate that while simpler models like Naïve Bayes and k-NN can be computationally efficient, they may not always capture the complexity of image data as effectively as neural networks.

## Conclusion
Neural networks, with their ability to learn complex patterns, proved to be the best performing model for this image classification task. However, the simplicity and efficiency of Naïve Bayes and k-NN make them suitable for other types of classification problems where the data may not be as complex.

## Credits

Special thanks to [Alkın Er](https://github.com/alkiner) for his contributions to the Naïve Bayes and k-NN models.


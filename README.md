# Animal-Classification-2022
A course project 2022

# Deep Learning Computer Vision Project

## Introduction
This project focuses on utilizing deep learning techniques for image classification. The dataset used in this project contains images of various animals. The goal is to classify each image into its respective animal category. 

## Problem Statement
Given a dataset consisting of animal images, the task is to develop a deep learning model that can accurately classify each image into one of the predefined animal categories.

## Methodology
### Data Collection and Preparation
- The dataset was obtained from a ZIP file containing images of different animals.
- The data extraction process involved unzipping the provided ZIP file to access the image files.

### Data Preprocessing
- Images were resized to a uniform size of 256x256 pixels to ensure consistency in input dimensions.
- Normalization was performed by scaling pixel values to the range [0, 1].

### Model Development
- VGG16, a pre-trained convolutional neural network (CNN) model, was employed as the base architecture.
- The pre-trained VGG16 model was fine-tuned by adding custom dense layers to adapt it to the specific classification task.
- The model was compiled with a sparse categorical cross-entropy loss function and the Adam optimizer.

### Model Training
- The dataset was split into training, validation, and testing sets.
- Training was conducted using the compiled VGG16 model with early stopping to prevent overfitting.
- Cross-validation using K-fold was employed to evaluate model performance and generalize its effectiveness.

### Model Evaluation
- Performance metrics such as accuracy, precision, recall, and F1 score were computed to assess the model's effectiveness.
- Confusion matrix visualization was utilized to gain insights into classification performance across different animal categories.

## Results
- The trained model achieved an overall accuracy of approximately 70% on the test dataset.
- Evaluation metrics indicated good performance in terms of precision, recall, and F1 score for most animal categories.
- Cross-validation results demonstrated consistent performance across multiple folds, indicating the model's robustness.

## Conclusion
The developed deep learning model based on the VGG16 architecture effectively classified animal images with high accuracy. Further optimization and fine-tuning could potentially enhance the model's performance for real-world applications.

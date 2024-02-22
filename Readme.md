# Chest X-ray Pneumonia Detection using Convolutional Neural Networks

This repository contains code for building and training a Convolutional Neural Network (CNN) to detect pneumonia from chest X-ray images. The dataset used in this example is sourced from [Cell](https://www.cell.com/cell/fulltext/S0092-8674(18)30154-5).

## Introduction

Pneumonia is a respiratory condition that inflames the air sacs in one or both lungs. Detecting pneumonia from medical images, such as chest X-rays, plays a crucial role in its diagnosis and treatment. Deep learning techniques, particularly CNNs, have shown promising results in automating this process.

## Setup and Data Loading

The code provided sets up the environment, including importing necessary libraries and connecting to a Google Cloud link to access the dataset. It then loads the chest X-ray data for training and testing, ensuring balanced representation between normal and pneumonia cases.

## Data Preprocessing

The data is preprocessed, mapping filenames to corresponding (image, label) pairs, where labels are encoded to indicate pneumonia or normal cases. The dataset is split into training and validation sets, and test data is prepared for evaluation.

## Model Architecture

The CNN model architecture is defined, comprising convolutional and dense layers. The architecture is inspired by a referenced article and is designed to extract features from chest X-ray images effectively.

## Addressing Data Imbalance

Due to an imbalance in the dataset, with more pneumonia cases than normal cases, class weighting is applied to balance the representation during training.

## Model Training

The model is trained using the defined architecture, with metrics such as precision, recall, and binary accuracy tracked to evaluate performance. Callbacks such as checkpoint saving and early stopping are employed to optimize training.

## Visualizing Model Performance

Training and validation metrics, including precision, recall, binary accuracy, and loss, are visualized to assess the model's performance over epochs.

## Evaluating Results

The trained model is evaluated on the test dataset, and the accuracy, precision, and recall are reported. Additionally, individual predictions on sample test images are made and presented.

## Conclusion

The provided code demonstrates the process of building and training a CNN for pneumonia detection from chest X-ray images. Further optimization and fine-tuning can be explored to improve model performance and generalizability.

For detailed implementation and execution, refer to the code provided in the repository.
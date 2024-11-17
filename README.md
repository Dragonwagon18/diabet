## RetiNet
RetiNet is a custom Convolutional Neural Network (CNN) designed for image classification tasks. This lightweight architecture includes multiple convolutional layers with batch normalization, ReLU activations, and dropout for regularization. The network is tailored for binary classification problems, making it suitable for applications like medical image analysis or small-scale datasets.


## Features
• Sequential Design: Stacked convolutional layers for feature extraction.
• Regularization: Includes batch normalization and dropout to prevent overfitting.
• Compact and Efficient: Optimized for smaller datasets and binary classification tasks.
• Customizable: Easily adaptable to other datasets and tasks with minor adjustments.

## Architecture
• Convolutional Layers: Eight layers with consistent kernel sizes and ReLU activations.
• Pooling: Single max-pooling layer for downsampling.
• Fully Connected Layers: Three layers for feature integration and output generation.
• Binary Output: Final sigmoid activation for classification.

## About the dataset
The Dataset contains images of images of left and right eye.
More info can be found here:https://www.kaggle.com/c/diabetic-retinopathy-detection/data

## Data Preprocessing
As the images had noise so, i removed them by cropping the images, also there was class imbalance problem, so i removed it by data augmentation.

## About Implementation
Here I have implemented diabetic retinopathy detection on Kaggle Dataset.There are two implementation in this repository:

### 1. Binary classification:
In bin_retinet.py , the model predicts whether a person has diabetic retinopathy or not.

### 2.Multiclass classification:
In multi_retinet.py the model predicts whether a person has :
0 - No DR
1 - Mild
2 - Moderate
3 - Severe
4 - Proliferative DR

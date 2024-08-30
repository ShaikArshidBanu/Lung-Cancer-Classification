# Lung-Cancer-Classification

## Overview

This project aims to classify lung cancer using the IQ-OTH/NCCD lung cancer dataset. The classification is performed by enhancing image quality through various contrast enhancement techniques and extracting features using multiple deep learning architectures. The extracted features are then classified into three categories: benign, malignant, and normal, using a Support Vector Machine (SVM) classifier.

## Dataset

The dataset used for this project is the **IQ-OTH/NCCD lung cancer dataset**, which contains annotated images representing different types of lung cancer cases. The dataset includes:

- **Benign cases**
- **Malignant cases**
- **Normal cases**

## Image Preprocessing

To improve the quality of the input images, three contrast enhancement techniques were applied:

1. **Contrast Limited Adaptive Histogram Equalization (CLAHE)**: Enhances the local contrast of the images.
2. **Unsharp Masking**: Increases the sharpness of the images by enhancing edges.
3. **Contrast Stretching**: Adjusts the contrast of the images to improve visibility.

## Feature Extraction

Seven deep learning architectures were utilized for feature extraction from the enhanced images:

1. **LeNet-5**
2. **ResNet-50**
3. **DenseNet-121**
4. **Deep Neural Network (DNN)**
5. **Convolutional Neural Network (CNN)**
6. **VGG-16**
7. **GoogLeNet (InceptionV3)**

Each model was trained on the processed images to extract relevant features that would aid in accurate classification.

## Classification

The extracted features from the deep learning models were input into a Support Vector Machine (SVM) classifier, which is known for its effectiveness in high-dimensional spaces. The SVM classifier was trained to categorize the images into three classes: 

- **Benign**
- **Malignant**
- **Normal**

## Results

Among the various experiments conducted, the combination of CLAHE-enhanced images with the features extracted using the DNN model and classified with the SVM classifier achieved the highest test accuracy of **96%**. This demonstrates the effectiveness of using advanced preprocessing and feature extraction techniques for lung cancer classification.


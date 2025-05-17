# Brain Disease Detection Using ResNet50

## Project Overview

This project focuses on the automated detection and classification of brain diseases, specifically Alzheimer's disease, Parkinson's disease, and brain tumors, using deep learning. By utilizing the ResNet50 convolutional neural network and transfer learning techniques, the system analyzes MRI brain images and classifies them into one of the aforementioned conditions or identifies them as healthy. A web-based user interface facilitates real-time predictions, making the tool suitable for potential use in hospitals, diagnostic centers, and research institutions.

## Objectives

* Automatically detect and classify Alzheimer's disease, Parkinson's disease, and brain tumors.
* Utilize transfer learning to enhance performance with limited datasets.
* Apply advanced preprocessing techniques to improve image quality and model performance.
* Develop a web-based platform for real-time diagnosis and usability.
* Achieve high accuracy and robust classification performance.

## Dataset Summary

The system is trained on publicly available MRI datasets:

* **Alzheimer's** (OASIS): 86,390 images across 4 stages.
* **Parkinson's** (Kaggle): 15,032 images across 5 stages.
* **Brain Tumors** (Kaggle): 5,712 images across 4 tumor classes.

Total dataset size: 103,553 MRI images. All data was anonymized and ethically sourced.

## Preprocessing Techniques

* **Bias Field Correction**: N4ITK for intensity inhomogeneity correction.
* **Spatial Smoothing**: Gaussian filtering for noise reduction.
* **Spatial Normalization**: Aligning scans to MNI template.
* **Nuisance Regression**: Removing scanner noise and non-brain signals.

## Model Architecture

* **Base Network**: ResNet50 (pretrained on ImageNet)
* **Input Size**: 224x224 RGB images
* **Optimizer**: Adam / SGD
* **Loss Function**: CrossEntropyLoss
* **Performance Metrics**: Accuracy, F1-Score, Precision, Recall, Confusion Matrix

## Training and Results

* **Initial Accuracy**: 71%
* **Final Accuracy**: 99% (after tuning hyperparameters like learning rate, dropout, weight decay)
* **Evaluation**: Robust performance on all classes, high generalization ability, confusion matrix and F1-scores confirm strong classification.

## Deployment

The model is integrated into a user-friendly web interface:

* **Frontend**: HTML, CSS, JavaScript
* **Backend**: Python (Flask or similar), handling model inference
* **Functionality**: Upload MRI, receive disease prediction in real-time

## Real-World Applications

* Assists clinicians in early-stage diagnosis.
* Supports medical learning and research.
* Useful in low-resource environments with limited radiological expertise.

## Limitations and Future Work

* Trained on structural MRI only (no severity staging or segmentation).
* Requires further validation on diverse, real-world clinical data.
* Future scope includes multi-modal imaging support, mobile deployment, and integration into telemedicine systems.
* 
---

For more information, please refer to the full project report included in the repository.

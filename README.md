# Deep-Learning-Based-Detection-of-Alzheimer-s-Brain-Tumor-and-Parkinson-s-Disease
## Brain Disease Classification Using Deep Learning
### Overview
This project focuses on the automated classification of brain diseases—Alzheimer's Disease, Parkinson's Disease, and Brain Tumors—using deep learning techniques applied to medical imaging data. Early and accurate detection of such neurological disorders can play a crucial role in timely intervention and treatment planning.
The project involves developing, training, and evaluating a Convolutional Neural Network (CNN) model that can analyze brain MRI images and classify them into one of the following categories:

Alzheimer's Disease
Parkinson's Disease
Brain Tumor

### Dataset

The project uses publicly available datasets from sources such as:
Kaggle 
Neuroimaging Archives (e.g., ADNI, TCIA)

Each image is preprocessed (resized, normalized) and labeled according to the corresponding condition. The dataset is split into training, validation, and test sets to evaluate model performance.

### Features

Deep learning model trained using PyTorch
Data preprocessing and augmentation to improve model generalization
Multi-class classification output with softmax activation
Performance metrics: accuracy, confusion matrix, precision, recall, F1-score
Visualization of training history and predictions

### Website (local) 

A simple web interface allows users to:
Upload a brain MRI image
View the model's predicted disease class
Understand confidence scores for each category

### Model Architecture

The current model uses pre-trained models (ResNet50) to improve accuracy and reduce training time.

### Evaluation Results

| Class       | Precision | Recall | F1-Score |
| ----------- | --------- | ------ | -------- |
| Alzheimer's | 0.95      | 0.94   | 0.94     |
| Parkinson's | 0.91      | 0.90   | 0.90     |
| Brain Tumor | 0.93      | 0.92   | 0.92     |
| Normal      | 0.96      | 0.97   | 0.96     |


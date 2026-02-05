# ✏️ MNIST Digit Recognition using Machine Learning

## Project Overview
This project implements a machine learning model to classify handwritten digits (0–9) using the **MNIST dataset**. The model leverages a **Convolutional Neural Network (CNN)** for high accuracy in recognizing digits from images.

## Objectives
- Preprocess image data  
- Normalize pixel values and reshape for CNN input  
- Train a supervised CNN model  
- Classify digits 0–9 accurately  
- Evaluate model performance using accuracy and visualization  

## Dataset
**Dataset:** MNIST Handwritten Digits Dataset  
**Image size:** 28x28 pixels (grayscale)  
**Number of classes:** 10 (digits 0–9)  
**Source:** Loaded directly from Keras datasets module  

## Technologies & Libraries
- Python, NumPy, Matplotlib  
- TensorFlow / Keras  

## Methodology

### 1. Data Preprocessing
- Normalized pixel values to the 0–1 range  
- Reshaped images to add a channel dimension `(28,28,1)`  
- One-hot encoded labels for 10 classes  

### 2. Model Architecture
- **Conv2D:** 32 filters, 3x3 kernel, ReLU activation  
- **MaxPooling2D:** 2x2  
- **Conv2D:** 64 filters, 3x3 kernel, ReLU activation  
- **MaxPooling2D:** 2x2  
- **Flatten → Dense:** 128 units, ReLU  
- **Output Dense:** 10 units, Softmax activation  

### 3. Model Training
- Optimizer: **Adam**  
- Loss function: **Categorical Crossentropy**  
- Epochs: 5 (adjustable)  
- Batch size: 128  
- Dataset split: 90% training, 10% validation  

### 4. Model Evaluation
- **Typical Test Accuracy:** ~98–99%  
- Optional visualization of predictions using Matplotlib  

## Author
**Tayyba Waheed**  
Machine Learning Intern

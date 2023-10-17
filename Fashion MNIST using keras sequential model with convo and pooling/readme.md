# Fashion MNIST Image Classification

This repository contains Python code for a Convolutional Neural Network (CNN) model that classifies images from the Fashion MNIST dataset. The Fashion MNIST dataset is available in TensorFlow and Keras libraries, allowing you to import it without the need for separate downloads. It consists of grayscale clothing images with a resolution of 28x28 pixels, each associated with one of ten classes:

1. T-shirt/top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle boot

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Code Structure](#code-structure)
- [Usage](#usage)
- [Model Summary](#model-summary)


## Introduction

The provided code includes Python scripts for loading and preparing the Fashion MNIST dataset, defining a CNN model, and running a test harness to evaluate the model's performance. Additionally, it allows you to make predictions on new images.

## Prerequisites

Before running the code, ensure that you have the following Python libraries installed:

- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-Learn

You can install these libraries using pip:

```bash
pip install tensorflow keras numpy matplotlib scikit-learn
```

## Code Structure

The code is structured into the following sections:

### 1. Load Dataset
The `load_dataset` function is responsible for loading the Fashion MNIST dataset. It reshapes the data into a single-channel format and one-hot encodes the target labels for training.

### 2. Scale Pixels
The `prep_pixels` function converts pixel values from integers to floats and normalizes them to a range between 0 and 1.

### 3. Define CNN Model
The `define_model` function creates a Sequential model with convolutional layers, pooling layers, and dense layers. This architecture is specifically designed for image classification, and the details are provided within the function.

### 4. Run Test Harness
The `run_test_harness` function manages the training process of the model. It loads the dataset, prepares pixel data, defines the model, fits the model to the data, and saves the model for future use.

### 5. Making Predictions
This section of the code demonstrates how to load a sample image, preprocess it, and employ the trained model for making predictions. You can replace 'sample_image.png' with the path to your image for classification.

## Usage

To utilize the code, follow these steps:

1. Clone this repository or download the code files.

2. Ensure that you have the required libraries installed, as mentioned in the prerequisites.

3. Execute the `run_test_harness` function to train the model and save it:

   ```python
   run_test_harness()
   ```

## Model Summary

The CNN model used in this code is specialized for image classification and has the following architecture:

- Input Layer: 28x28 grayscale images
- Convolutional Layer: 32 filters with a 3x3 kernel and ReLU activation
- Max Pooling Layer: 2x2 pool size
- Flatten Layer
- Dense Layer: 100 units with ReLU activation
- Output Layer: 10 units with softmax activation

The model is compiled using stochastic gradient descent (SGD) as the optimizer, and categorical cross-entropy is selected as the loss function for multiclass classification.

A visual summary of the model is saved as 'CNN_seq.png'.

You are encouraged to explore, customize, and apply this code for your image classification projects!

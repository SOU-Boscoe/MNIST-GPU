# MNIST-GPU

# PyTorch MNIST Training Performance Benchmark

A comprehensive comparison of PyTorch model training performance across different platforms and hardware configurations using the MNIST dataset.

## Project Overview

This project benchmarks the time required to train a neural network model on the MNIST dataset for 50 epochs across various computing environments. Our goal is to provide insights into the performance characteristics of different platforms commonly used in machine learning development and research.

## Platforms Tested

- **Keras on JupyterHub** - Cloud-based notebook environment with Keras/TensorFlow backend
- **Kaggle Notebooks** - Kaggle's free notebook environment
- **M1 MacBook (Bare Metal)** - Apple Silicon M1 chip with native PyTorch optimization
- **TensorFlow on Google Colab** - Google's free cloud notebook platform
- **GPU on Jetstream** - NSF-funded cloud computing platform with dedicated GPU resources

## Dataset

**MNIST (Modified National Institute of Standards and Technology)**
- 70,000 grayscale images of handwritten digits (0-9)
- Training set: 60,000 images
- Test set: 10,000 images
- Image dimensions: 28x28 pixels

## Model Architecture

The benchmark uses a standardized neural network architecture across all platforms to ensure fair comparison:

## Training Configuration

- **Epochs**: 50
- **Batch Size**: 64
- **Optimizer**: Adam (lr=0.001)
- **Loss Function**: CrossEntropyLoss
- **Metrics Tracked**: Training time, accuracy, loss
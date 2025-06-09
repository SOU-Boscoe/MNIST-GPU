# MNIST-GPU

## Notebook description

This notebook shows how to check the GPU, load and train the MNIST dataset and model, with training times and how the architecture works.
We also show the time required to train a CNN (convolutional neural network) model on the MNIST dataset for 50 epochs across various computing environments. Our goal is to show when a GPU is useful for performance (and sometimes necessary)

## Platforms Tested

- **Keras on JupyterHub** - Cloud-based notebook environment with Keras/TensorFlow backend
- **Kaggle Notebooks** - Kaggle's free notebook environment
- **M1 MacBook (Bare Metal)** - Apple Silicon M1 chip with native PyTorch optimization
- **TensorFlow on Google Colab** - Google's cloud notebook platform
- **GPU on Jetstream2** - NAIRR's NSF-funded cloud computing platform with dedicated GPU resources

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
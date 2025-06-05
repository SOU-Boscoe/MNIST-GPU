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

## Results Summary

*Note: Results will be updated as benchmarks are completed*

| Platform | Hardware | Training Time (50 epochs) | Final Accuracy | Notes |
|----------|----------|---------------------------|----------------|-------|
| Keras/JupyterHub | CPU | TBD | TBD | Cloud CPU |
| Kaggle | CPU | TBD | TBD | |
| M1 MacBook | M1 GPU | TBD | TBD | Native Apple Silicon |
| Colab | CPU | TBD | TBD |  |
| Jetstream | GPU | TBD | TBD | Dedicated research GPU |

## Key Findings

*To be updated upon completion of benchmarks*

- Performance comparison across different hardware accelerators
- Impact of cloud vs local execution
- Resource utilization patterns
- Cost-effectiveness analysis

## Methodology

### Timing Measurement

### Standardization Measures
- Identical model architecture across all platforms
- Same hyperparameters and training configuration
- Consistent random seed for reproducible results
- Standardized data preprocessing pipeline

## Acknowledgments

- MNIST dataset
    - http://yann.lecun.com/exdb/mnist/
- JetStream
    - Stewart, C.A., Cockerill, T.M., Foster, I., Hancock, D., Merchant, N., Skidmore, E., Stanzione, D., Taylor, J., Tuecke, S., Turner, G., Vaughn, M., and Gaffney, N.I., “Jetstream: a self-provisioned, scalable science and engineering cloud environment.” 2015, In Proceedings of the 2015 XSEDE Conference: Scientific Advancements Enabled by Enhanced Cyberinfrastructure. St. Louis, Missouri. ACM: 2792774. p. 1-8. DOI: https://dl.acm.org/doi/10.1145/2792745.2792774
    - John Towns, Timothy Cockerill, Maytal Dahan, Ian Foster, Kelly Gaither, Andrew Grimshaw, Victor Hazlewood, Scott Lathrop, Dave Lifka, Gregory D. Peterson, Ralph Roskies, J. Ray Scott, Nancy Wilkins-Diehr, “XSEDE: Accelerating Scientific Discovery,” Computing in Science & Engineering, vol.16, no. 5, pp. 62–74, Sept.–Oct. 2014. DOI: https://ieeexplore.ieee.org/document/6866038

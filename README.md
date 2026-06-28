# Denoising Autoencoder on MNIST Dataset

## Overview

This project implements a **Denoising Autoencoder (DAE)** using TensorFlow/Keras to remove noise from handwritten digit images in the MNIST dataset. The model is trained using noisy images as input and clean images as target outputs.

## Objectives

- Load and preprocess the MNIST dataset.
- Add artificial Gaussian noise to the images.
- Build and train a Denoising Autoencoder.
- Generate denoised images from noisy inputs.
- Evaluate the model's reconstruction performance.

## Dataset

The MNIST dataset contains:
- 60,000 training images
- 10,000 testing images
- Grayscale handwritten digits (0–9)
- Image size: 28 × 28 pixels

## Methodology

### Data Preprocessing
- Loaded the MNIST dataset.
- Normalized pixel values to the range [0,1].
- Reshaped images for convolutional neural network processing.

### Noise Addition
- Added Gaussian noise to create noisy versions of the images.
- Clipped pixel values to maintain valid image ranges.

### Model Architecture
The Denoising Autoencoder consists of:

#### Encoder
- Conv2D Layer
- MaxPooling2D Layer
- Conv2D Layer
- MaxPooling2D Layer

#### Decoder
- Conv2D Layer
- UpSampling2D Layer
- Conv2D Layer
- UpSampling2D Layer
- Output Conv2D Layer (Sigmoid Activation)

### Training
- Input: Noisy Images
- Target: Clean Images
- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Epochs: 10
- Batch Size: 128

## Results

- Successfully trained the Denoising Autoencoder.
- Training and validation loss decreased consistently.
- The model effectively removed noise while preserving digit structure.
- Generated clear reconstructed images from noisy inputs.

## Observations

- The model learned meaningful image representations.
- Denoised outputs were significantly cleaner than noisy inputs.
- Validation loss closely followed training loss, indicating good generalization.

## Challenges

- Selecting an appropriate noise level.
- Balancing image reconstruction quality and noise removal.
- Managing training time and computational resources.

## Conclusion

The Denoising Autoencoder successfully reconstructed clean handwritten digit images from noisy inputs. This project demonstrates the effectiveness of autoencoders for image denoising and image restoration tasks.

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib

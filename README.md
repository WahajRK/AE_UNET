# Understanding AutoEncoders and U-Net

## Overview
This repository explores Auto-Encoders and U-Net architectures for unsupervised learning, focusing on image reconstruction and defect detection. The project utilizes Pyramid Location Network (Pylon) images with RESNET50 to enhance feature extraction and improve accuracy.

## Architecture
- **Encoder:** Compresses input images into a lower-dimensional latent representation.
- **Decoder:** Reconstructs the input image from the encoded representation.
- **U-Net:** An extension of Autoencoders with skip connections for better feature retention.

## Features
- Implements convolutional blocks with batch normalization and activation functions.
- Supports both Autoencoder-based reconstruction and U-Net segmentation.
- Leverages deep learning for dimensionality reduction and feature learning.

## Use Cases
- Image Denoising
- Anomaly & Defect Detection
- Feature Extraction for Classification

## Installation & Usage
### **Installation**
```bash
# Clone the repository
git clone git@github.com:WahajRK/AE_UNET.git

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt
### **Usage**
```bash
# Train the Autoencoder
python ae_unet.py
```
This script loads images from the `Pylon_images/DIN_Gray` directory, preprocesses them, and trains an autoencoder model. The trained model will be saved as `autoencoder_pylon_grayscale_img_5epochs.h5`.



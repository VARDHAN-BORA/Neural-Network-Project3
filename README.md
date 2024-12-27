# Bird Sound Image Segmentation with UNet

## Overview
This project is an implementation of an **Image Segmentation Model** using PyTorch, focusing on the segmentation of bird sound spectrogram images. The project employs a **UNet architecture** for semantic segmentation. The dataset used consists of spectrogram images and their respective masks. The training, validation, and testing processes are performed on the Bird Sound Dataset.

## Features
- **UNet Architecture**: A powerful deep learning architecture designed for image segmentation.
- **Bird Sound Dataset**: Used spectrogram images for input and corresponding masks for output.
- **PyTorch Framework**: Leveraging PyTorch for model implementation and training.
- **Google Colab Integration**: The project is implemented and trained using Google Colab, with Google Drive integration for dataset handling.
- **Training and Validation Pipeline**: Includes metrics for training and validation loss.

## Dataset
The dataset contains:
- **Images**: Spectrograms representing bird sounds.
- **Masks**: Binary masks indicating the segmented regions in the spectrograms.

### Folder Structure:
- /dataset /train /images /masks /valid /images /masks /test /images /masks


### Data Transformations:
- Resizing all images and masks to 256x256 pixels.
- Converting images and masks to tensors.

## Model
The model is based on the **UNet architecture**:
- **Encoder**: A series of convolutional layers for feature extraction.
- **Decoder**: Up-convolutional layers with skip connections from the encoder for detailed segmentation.
- **Output Layer**: A single-channel output layer with a sigmoid activation for binary segmentation.

## Training
- The training process involves minimizing a binary cross-entropy loss function.
- The dataset is split into training, validation, and testing sets.
- The best model is saved based on the lowest validation loss.

### Metrics:
- **Training Loss**
- **Validation Loss**

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/VARDHAN-BORA/Neural-Network-Project3.git


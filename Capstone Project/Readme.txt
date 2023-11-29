# Building Classification in Rural Areas using Deep Learning

## Project Overview:

This project focuses on developing a robust image classification system for drones, specifically designed for rural areas. The objective is to accurately classify drone-captured images into two categories: "mud house" and "cattle shed." The utilization of deep learning and computer vision techniques contributes to efficient monitoring and assessment of rural infrastructure, providing valuable insights for development and resource allocation.

## Data Collection:

- **Large TIF Drone Image:** A comprehensive drone image of a village.
- **Cropped RGB Images:** Focused images of houses and cattle sheds.
- **Labeling Process:** Images labeled as "Mud House" or "Cattle Shed."
- **Data Imbalance:** 198 mud houses, 247 cattle sheds.

## Data Handling:

- **Google Drive:** Dataset uploaded for accessibility.
- **Google Colab:** Utilized for training due to GPU limitations.
- **Limited GPU Resources:** Acknowledged in the documentation.

## Data Preprocessing:

- **Normalization:** Ensured consistent data scaling.
- **Data Imbalance Handling:** Employed SMOT and Keras's methods.
- **Data Augmentation:** Enhanced dataset due to its small size.

## Model Architecture - CNN:

- **Architecture:** Custom CNN model using Keras.
- **Layers:** Three Conv2D layers, MaxPooling2D layers, Flattening layer, Dense layer (256 neurons, ReLU activation).
- **Compilation:** Adam optimizer; Input shape (256, 256, 3).

## Model Architecture - Transfer Learning (VGG16):

- **Utilization:** Pretrained VGG16 model.
- **Customization:** Top layers frozen; Custom layers added for classification.
- **Feature Extraction:** Leveraged CNN part of VGG16.
- **VGG16 Details:** 16 layers, including 13 convolutional layers and 3 fully connected layers; Trained on ImageNet dataset.

## Training Process:

- **Epochs:** Trained for 20 epochs.
- **Early Stopping:** Implemented to prevent overfitting.
- **Validation Data:** Used for assessing model performance.
- **Insights:** Comprehensive training insights for model selection and optimization.

## Web App Implementation:

- **Functionality:** Simple web app allowing user image selection and predicting building type.
- **Library:** Utilized a Python library for creating interactive web applications with minimal code.

## Achievements:

- Successfully classified rural building types: mud houses vs. cattle sheds.
- Overcame data imbalance and GPU limitations using Google Colab.
- Employed custom CNN and VGG16 transfer learning for robust models.
- Evaluation metrics and confusion matrices validated model accuracy.

## Areas for Improvement:

- Expand dataset for enhanced model generalization.
- Explore additional model architectures for performance improvement.
- Refine the web app for a more user-friendly experience.

Feel free to explore the code and documentation for a detailed understanding of the project.

# Time Series Classification of Discrete-Time Chaotic Systems Using CNNs

This repository provides an implementation of deep learning–based classification of
**discrete-time chaotic systems** using **convolutional neural networks (CNNs)** and
traditional machine learning classifiers.

The project follows the methodology presented in the paper:

> Akmeşe, Ö. F., Emin, B., Alaca, Y., Karaca, Y., & Akgül, A.  
> *The Time Series Classification of Discrete-Time Chaotic Systems Using Deep Learning Approaches*  
> Mathematics, 12(19), 3052, 2024.  
> DOI: 10.3390/math12193052

---

## Overview

Discrete-time chaotic systems exhibit nonlinear and unpredictable behavior, making
their classification a challenging task.  
This project addresses this problem by:

- Generating time series from nine discrete-time chaotic systems
- Converting time series into image representations
- Extracting deep features using CNN architectures
- Performing classification using machine learning algorithms

The objective is to identify the underlying chaotic system from its time-series dynamics.

---

## Chaotic Systems Included

The dataset is generated from the following nine discrete-time chaotic maps:

1. Logistic Map  
2. Sine Map  
3. Tent Map  
4. Cubic Map  
5. Pinchers Map  
6. Spence Map  
7. Cusp Map  
8. Ricker’s Population Model  
9. Gauss Map  

Each system is simulated using multiple:
- Control parameters  
- Initial conditions  
- Iteration lengths  

This ensures dataset diversity and balanced class representation.

---

## Dataset Description

- Total images: **10,080**
- Images per system: **1,120**
- Image size: **256 × 256**
- Format: Grayscale images (no gridlines)

The dataset is generated programmatically from the mathematical equations of the
chaotic systems.

**Note:**  
The dataset is not included directly in this repository.  
All scripts required to regenerate the dataset are provided.


## CNN Models Used
The following convolutional neural network architectures are used as feature extractors
via transfer learning:

- DenseNet121
- VGG16
- VGG19
- InceptionV3
- MobileNetV2
- Xception

These CNN models are employed to learn high-level representations from
time-series images before classification

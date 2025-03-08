# Project 'Face Detection'

---

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Description

I have built a **Convolutional Neural Network (CNN)** using TensorFlow library in 
order to fit a model to detect face position in an image. 

### Model details
- **Optimizer:** Adam
- **Loss:** Mean Squared Error
- **Layers**
  - **Input of 256x256x3** (RGB image 256x256)
  - **2D Convolution** (64 filters of 3x3, activation **'relu'**)
  - **2D MaxPooling** (pool size 2x2)
  - **2D Convolution** (64 filters of 3x3, activation **'relu'**)
  - **2D MaxPooling** (pool size 2x2)
  - **2D Convolution** (128 filters of 3x3, activation **'relu'**)
  - **2D MaxPooling** (pool size 2x2)
  - **2D Convolution** (128 filters of 3x3, activation **'relu'**)
  - **2D MaxPooling** (pool size 2x2)
  - **Flatten**
  - **Dense layer** (128 units, activation **'relu'**)
  - **Dense layer** (4 units, activation **'linear'**)
- **Params**
  - **Total params:** 3,472,068 (13.24 MB)
  - **Trainable params:** 3,472,068 (13.24 MB)
- **Train details**
  - 10 epochs
  - batch size of 32 units
- **Metrics**
  - **on training set:** 
    - **accuracy:** 0.83
    - **loss:** 522
  - **on validation set:**
    - **accuracy:** 0.65
    - **loss:** 1128
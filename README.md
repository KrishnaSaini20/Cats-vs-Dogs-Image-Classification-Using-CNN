# Cats vs Dogs Image Classification Using CNN

## Overview

This project implements an image classification model using Convolutional Neural Networks (CNN) to distinguish between images of cats and dogs.

The model is developed using TensorFlow and Keras. It learns visual features such as shapes, textures, and patterns from images to classify them into two categories: Cat and Dog.

The project demonstrates the application of deep learning and computer vision for binary image classification.

## Features

- Image dataset loading using TensorFlow.
- Image resizing to 256 × 256 pixels.
- Image normalization.
- CNN-based image classification.
- Batch Normalization for stable training.
- Max Pooling for dimensionality reduction.
- Dropout for regularization.
- Model training and validation.
- Prediction on custom images.

## Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib

## Dataset

The project uses the Dogs vs Cats dataset from Kaggle.

Dataset: https://www.kaggle.com/datasets/salader/dogsvscats

Dataset distribution:

| Dataset | Number of Images |
|---|---:|
| Training | 20,000 |
| Validation | 5,000 |
| Total | 25,000 |

Image dimensions: 256 × 256 pixels.

## CNN Architecture

The model consists of the following layers:

1. **Convolutional Layers:** Extract visual features from input images using 32, 64, and 128 filters.
2. **Batch Normalization:** Helps stabilize the training process.
3. **Max Pooling:** Reduces spatial dimensions and computational complexity.
4. **Flatten Layer:** Converts feature maps into a one-dimensional vector.
5. **Dense Layers:** Learn higher-level representations for classification.
6. **Dropout:** Helps reduce overfitting.
7. **Output Layer:** Uses a sigmoid activation function for binary classification.

## Model Configuration

| Parameter | Value |
|---|---|
| Input Image Size | 256 × 256 × 3 |
| Batch Size | 32 |
| Optimizer | Adam |
| Loss Function | Binary Crossentropy |
| Evaluation Metric | Accuracy |
| Epochs | 10 |
| Output Activation | Sigmoid |

## Model Performance

Recorded results after 10 epochs:

| Metric | Result |
|---|---:|
| Training Accuracy | 94.85% |
| Validation Accuracy | 82.84% |

The training and validation accuracy curves indicate a gap between training and validation performance, suggesting overfitting.

## Project Workflow

1. Download and extract the dataset.
2. Load training and validation images.
3. Resize images to 256 × 256.
4. Normalize pixel values between 0 and 1.
5. Build the CNN architecture.
6. Compile the model using Adam optimizer and binary crossentropy.
7. Train the model for 10 epochs.
8. Evaluate training and validation performance.
9. Visualize accuracy and loss curves.
10. Predict whether custom images contain a cat or a dog.

## Installation

Clone the repository:

```bash
git clone https://github.com/USERNAME/Cats-vs-Dogs-CNN-Classification.git
```

Navigate to the project directory:

```bash
cd Cats-vs-Dogs-CNN-Classification
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `cats_vs_dogs.ipynb` and execute the cells sequentially.

## Future Improvements

- Apply data augmentation to improve generalization.
- Use Early Stopping to prevent unnecessary training.
- Experiment with L1/L2 regularization.
- Improve model performance using transfer learning with VGG16 or MobileNet.
- Save and load the trained model.
- Develop a web interface for real-time image classification.

## Author

**Your Name**

GitHub: https://github.com/USERNAME

---

*This project was developed as a practical implementation of Convolutional Neural Networks and deep learning for image classification.*

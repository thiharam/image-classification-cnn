# Image Classification Using Convolutional Neural Networks (CNN)

## Project Overview

This project implements an image classification model using Deep Learning and Convolutional Neural Networks (CNNs) with TensorFlow and Keras.

The objective is to develop a model capable of classifying images into 10 different categories using the CIFAR-10 dataset.

This project explores the fundamental concepts of Computer Vision, image preprocessing, CNN architecture, model training, and performance evaluation.

## Problem Statement

Image classification is a fundamental task in Computer Vision. It involves identifying and assigning a predefined category to an image based on its visual features.

The goal of this project is to develop a CNN-based model that can automatically identify the category of an input image.

## Dataset

**Dataset:** CIFAR-10

The CIFAR-10 dataset contains 60,000 colour images across 10 different classes.

| Dataset | Number of images |
|---|---:|
| Training dataset | 50,000 |
| Testing dataset | 10,000 |
| Total | 60,000 |

Each image has a resolution of 32 × 32 pixels with three RGB colour channels.

### Image Categories

1. Airplane
2. Automobile
3. Bird
4. Cat
5. Deer
6. Dog
7. Frog
8. Horse
9. Ship
10. Truck

The dataset is loaded directly using the TensorFlow/Keras dataset API.

## Technologies and Tools

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab / Jupyter Notebook

## Project Workflow

The project follows a standard Deep Learning workflow.

### 1. Environment Setup
- Configure the Python environment.
- Import the required libraries and frameworks.

### 2. Dataset Loading and Exploration
- Load the CIFAR-10 dataset.
- Explore image dimensions and pixel values.
- Visualize sample images and their corresponding labels.

### 3. Image Preprocessing
- Convert pixel values into floating-point numbers.
- Normalize RGB pixel values from 0–255 to 0–1.
- Separate the training, validation, and testing datasets.

### 4. CNN Model Development

Develop a Convolutional Neural Network consisting of:

| Layer | Configuration |
|---|---|
| Convolutional layer 1 | 32 filters, 3 × 3 kernel |
| Max pooling 1 | 2 × 2 |
| Convolutional layer 2 | 64 filters, 3 × 3 kernel |
| Max pooling 2 | 2 × 2 |
| Convolutional layer 3 | 128 filters, 3 × 3 kernel |
| Flatten | Feature vector |
| Dense layer | 128 neurons |
| Output layer | 10 neurons with Softmax |

### 5. Model Training
- Compile the CNN model using the Adam optimizer.
- Use Sparse Categorical Crossentropy as the loss function.
- Train the model using mini-batches.
- Monitor training and validation accuracy and loss.

### 6. Model Evaluation

Evaluate the trained model using:

- Accuracy
- Loss
- Precision
- Recall
- F1-score
- Confusion matrix

### 7. Model Improvement

Experiment with techniques to improve model generalization:

- Data augmentation
- Dropout regularization
- Hyperparameter adjustments
- Model architecture modifications

### 8. Prediction

Use the trained model to classify unseen images and compare predicted labels with actual labels.

## Model Architecture

The CNN extracts visual features through convolutional layers and uses fully connected layers to classify images into the 10 CIFAR-10 categories.

The architecture follows this general structure:

**Input Image → Convolution → ReLU → Max Pooling → Convolution → ReLU → Max Pooling → Convolution → Flatten → Dense → Softmax Output**

## Results and Evaluation

Results will be updated after completing model training and evaluation.

| Evaluation Metric | Baseline Model | Improved Model |
|---|---|---|
| Test Accuracy | To be updated | To be updated |
| Test Loss | To be updated | To be updated |
| Precision | To be updated | To be updated |
| Recall | To be updated | To be updated |
| F1-score | To be updated | To be updated |

### Performance Visualizations

The following visualizations will be included:

- Training and validation accuracy.
- Training and validation loss.
- Confusion matrix.
- Sample image predictions.

## Project Structure

```text
image-classification-cnn/
│
├── notebooks/
│   └── image_classification.ipynb
│
├── models/
│
├── results/
│   ├── accuracy.png
│   ├── loss.png
│   └── confusion_matrix.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/thiharam/image-classification-cnn.git
```

### 2. Navigate to the project directory

```bash
cd image-classification-cnn
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

Open the notebook located inside the `notebooks` directory using Jupyter Notebook or Google Colab.

### 5. Execute the notebook

Run the notebook cells sequentially to load the dataset, preprocess images, build the CNN, train the model, and evaluate its performance.

## Key Learning Outcomes

Through this project, the following concepts are explored:

- Digital image representation and RGB colour channels.
- Image preprocessing and normalization.
- Supervised learning.
- Convolutional Neural Networks.
- Convolution and feature extraction.
- Activation functions and pooling.
- Forward propagation and backpropagation.
- Model optimization and training.
- Model evaluation and performance metrics.
- Overfitting and regularization.
- Data augmentation.
- Model inference and prediction.

## Future Improvements

Potential extensions of this project include:

- Experimenting with deeper CNN architectures.
- Implementing transfer learning using pretrained models such as ResNet and MobileNet.
- Exploring different image augmentation techniques.
- Comparing different optimizers and hyperparameters.
- Developing a simple web application for image classification.
- Exploring image classification using RGB and thermal imaging data.

## References

- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
- [TensorFlow Documentation](https://www.tensorflow.org/)
- [Keras Documentation](https://keras.io/)
- [Scikit-learn Documentation](https://scikit-learn.org/)

---

**Project Category:** Deep Learning / Computer Vision

**Status:** In Progress

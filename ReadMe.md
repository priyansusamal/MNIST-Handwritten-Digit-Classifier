# Handwritten Digit Classifier using MNIST

A deep learning project that classifies handwritten digits from **0 to 9** using a Multi-Layer Perceptron (MLP) built with TensorFlow and Keras. The model is trained and evaluated on the MNIST dataset.

## Project Overview

The goal of this project is to build a neural network that can recognize handwritten digits from grayscale images. It demonstrates the fundamental concepts of neural networks, image preprocessing, model training, and performance evaluation.

## Tech Stack

- **Language:** Python
- **Deep Learning:** TensorFlow / Keras
- **Numerical Computing:** NumPy
- **Visualization:** Matplotlib
- **Evaluation:** Scikit-learn
- **Dataset:** MNIST

## Dataset

The MNIST dataset contains 70,000 grayscale images of handwritten digits:

- Training set: 60,000 images
- Test set: 10,000 images
- Image dimensions: 28 × 28 pixels
- Classes: 10 digits (0–9)

Pixel values are normalized from the range 0–255 to 0–1 before training.

## Model Architecture

The primary model is a Multi-Layer Perceptron (MLP) implemented using `tf.keras.Sequential`.

| Layer | Configuration |
|---|---|
| Input | 28 × 28 grayscale image |
| Flatten | Converts the image into 784 features |
| Hidden layer | 128 neurons, ReLU activation |
| Output layer | 10 neurons, Softmax activation |

### Training Configuration

- Optimizer: Adam
- Loss function: Sparse categorical cross-entropy
- Batch size: 32
- Epochs: 5
- Validation split: 10%

A smaller MLP with 64 hidden neurons is also trained to experiment with model architecture and compare performance.

## Features

- Loads the MNIST dataset using TensorFlow/Keras.
- Visualizes sample images from all ten digit classes.
- Preprocesses and normalizes image data.
- Builds and trains an MLP neural network.
- Evaluates performance on unseen test images.
- Plots training and validation accuracy and loss.
- Generates a confusion matrix to analyze classification performance.
- Compares two MLP architectures.

## Project Structure

```text
mnist-handwritten-digit-classifier/
│
├── AIML_Recruitment_MNIST.ipynb
├── README.md
└── requirements.txt
```

## Installation and Usage

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/mnist-handwritten-digit-classifier.git
cd mnist-handwritten-digit-classifier
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

Open `AIML_Recruitment_MNIST.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab and execute the cells in order.

The MNIST dataset will be downloaded automatically by TensorFlow when required.

## Requirements

Create a `requirements.txt` file containing:

```text
tensorflow
numpy
matplotlib
scikit-learn
jupyter
```

## Results

The model is evaluated on the MNIST test dataset using test loss and classification accuracy.

- **Test Accuracy:** [Add your actual test accuracy here]
- **Test Loss:** [Add your actual test loss here]

The notebook also includes training and validation curves, a confusion matrix, and an experimental model comparison.

## Learning Outcomes

- Understanding the fundamentals of artificial neural networks.
- Preprocessing image data for machine learning.
- Implementing an MLP using TensorFlow/Keras.
- Training and evaluating a multiclass classification model.
- Visualizing learning performance and analyzing classification errors.
- Comparing neural network architectures.

## Future Improvements

- Implement a Convolutional Neural Network (CNN).
- Experiment with different numbers of hidden layers and neurons.
- Tune hyperparameters to improve accuracy.
- Save the trained model for future predictions.
- Build an interface for classifying user-drawn digits.

## Acknowledgements

The MNIST handwritten digit dataset is widely used for learning and experimenting with image classification and neural networks.

---

**Project:** Handwritten Digit Classifier  
**Framework:** TensorFlow / Keras

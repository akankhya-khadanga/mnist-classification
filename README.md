# MNIST Digit Classification

A simple neural network built with **TensorFlow/Keras** to classify handwritten digits from the MNIST dataset.

## Overview

The model takes **28×28 grayscale images** as input and predicts one of the 10 digits (0–9).

### Workflow

* Load the MNIST dataset
* Normalize pixel values to 0–1
* Build and train a neural network
* Evaluate predictions on test data
* Visualize training and validation performance

## Model Architecture

```text
28 × 28 Image
     ↓
  Flatten
     ↓
Dense(128, ReLU)
     ↓
Dense(10, Softmax)
     ↓
Predicted Digit
```

The `Flatten` layer converts each 28×28 image into 784 values.
The final Softmax layer produces probabilities for the 10 possible digits.

## Training

* **Optimizer:** Adam
* **Loss:** Sparse Categorical Crossentropy
* **Epochs:** 25
* **Validation Split:** 20%
* **Metric:** Accuracy

## Technologies

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn

## Project Structure

```text
MNIST-Digit-Classification/
├── mnist_classification.ipynb
└── README.md
```

## How to Run

```bash
pip install tensorflow numpy matplotlib scikit-learn
```

Open `mnist_classification.ipynb` in **Jupyter Notebook, Google Colab, or VS Code** and run the cells.

## What I Learned

This project helped me understand the basics of **neural networks, image preprocessing, activation functions, model training, multiclass classification, and evaluation**.

## Future Improvements

* Experiment with different network architectures
* Add a confusion matrix
* Compare the neural network with a CNN
* Tune model hyperparameters



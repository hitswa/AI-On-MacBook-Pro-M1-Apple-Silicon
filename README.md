# AI On MacBook Pro M1 Apple Silicon

Last Updated: `2025-04-15`

## Setup

First Install homebrew if already not installed

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

now Install required components

```bash
# install cmake
brew install cmake # required for installing dm-tree
brew install python@3.10
```

**Note:** Please stick to the choice of Python version necessary to implement and work with libraries

Let's begin the initialisation of project now

```bash
# clone the project
git clone https://github.com/hitswa/AI-On-MacBook-Pro-M1-Apple-Silicon.git
# go to project
cd AI-On-MacBook-Pro-M1-Apple-Silicon
# initiate environment
python3.10 -m venv .
# activate environment
source ./bin/activate
# upgrate pip and other tools
pip install --upgrade pip setuptools wheel
# already initiated requirements.txt and has specific versions of libraries we used
# python3.10 -m pip freeze > requirements.txt
# Install the required libraries
python3.10 -m pip install -r requirements.txt
# check if everything is installed
python -m pip list
```

## Learning Roadmap & Exercises

We’ll follow a structured path from basic neural networks to deep learning applications.

### 🔹 Phase 1: Understanding and Implementing a Single Neuron

- Concepts: Perceptron, Activation Functions, Forward Propagation, Gradient Descent
- Exercise 1: Implement a single neuron in Python using NumPy (without any deep learning libraries)

### 🔹 Phase 2: Building a Simple Neural Network

- Concepts: Multilayer Perceptron (MLP), Backpropagation
- Exercise 2: Build a simple 3-layer neural network using only NumPy

### 🔹 Phase 3: Using TensorFlow and PyTorch

- Concepts: TensorFlow & PyTorch basics, defining layers, training loops
- Exercise 3: Implement the same neural network using TensorFlow and PyTorch

### 🔹 Phase 4: Training on Real Data

- Concepts: Dataset preparation, Loss Functions, Optimizers
- Exercise 4: Train a neural network on the MNIST dataset (handwritten digit recognition)

### 🔹 Phase 5: Convolutional Neural Networks (CNNs)

- Concepts: Convolutions, Pooling, Feature Extraction
- Exercise 5: Implement a CNN for image classification

### 🔹 Phase 6: Advanced Topics

- Recurrent Neural Networks (RNNs), LSTMs, Transformers
- Exercise 6: Train an LSTM to predict text sequences
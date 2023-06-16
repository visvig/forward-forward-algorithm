# Forward-Forward Algorithm Implementation

This repository contains the Jupyter notebook for the implementation of Geoffrey Hinton's Forward-Forward Algorithm. MNIST fully connected The code is based on the work of Mohammad Pezeshki. The original code can be found [here](https://github.com/mohammadpz/pytorch_forward_forward).

## Introduction

The Forward-Forward Algorithm offers an alternative approach to training neural networks. It replaces the conventional forward and backward passes employed in backpropagation with two forward passes. The first pass uses positive or real data, while the second pass uses negative data. The algorithm equips each layer in the network with its own objective function, designed to maximize the goodness for positive data and minimize it for negative data.

## Repository Contents

The Jupyter notebook `ff-mnist-fully-connected.ipynb` consists of the following sections:

- **A. Function to Generate Negative Labels**: A helper function to generate negative labels for the training samples.
- **B. Function to Overlay Label onto Input Data**: A helper function to overlay the labels onto the input data.
- **C. Custom Network Class**: A class definition for creating the neural network.
- **D. Custom Layer Class**: A class definition for creating layers of the neural network.
- **E. Network Hyperparameters and Device Setup**: Setting up the hyperparameters and the device for training the network.
- **1. Load Data**: Loading the MNIST dataset for training and testing.
- **2. Create Network**: Creating an instance of the network.
- **3. Train the Network**: Training the network on the MNIST dataset.
- **4. Test the Network**: Testing the network on the test data of the MNIST dataset.

The Jupyter notebook `ff-cifar10-convnet.ipynb` is under work!

## Getting Started

To run this code, you will need:

- torch
- torchvision

The data for training and testing is automatically downloaded using torchvision's inbuilt functions.

## Running the Code

To run the notebook, start Jupyter Notebook in the repository directory, and then open the `ff-mnist-fully-connected.ipynb` or `ff-cifar10-convnet.ipynb` file.

## Contributions

Feel free to submit issues and enhancement requests.

## Acknowledgements

- Mohammad Pezeshki for the [initial implementation](https://github.com/mohammadpz/pytorch_forward_forward).
- Geoffrey Hinton for the [Forward-Forward Algorithm](https://arxiv.org/abs/2212.13345).

## License

This project is licensed under the MIT License.

# Neural-Network-Classifier-with-Multiclass-Classification-for-MNIST-dataset
This exercise will focus on training a neural network classifier for the MNIST dataset. The goal of this exercise is understanding the effect of overparameterization and dropout on the training performance and test accuracy. 

**Multiclass Neural Network: Softmax & Cross-Entropy Implementation**

This repository contains a manual, from-scratch implementation of a Multiclass Neural Network designed to classify the MNIST dataset.

**Key Technical Implementations**

Implemented the Softmax function at the output layer to transform raw scores into a probability distribution where all values sum to 1.

Replaced Mean Squared Error (MSE) with Cross-Entropy Loss. This improvement provides stronger gradients for incorrectly classified examples, leading to faster and more robust convergence compared to quadratic objectives.

Derived and implemented the combined gradient for the Softmax and Cross-Entropy layers.

**Experimental Results**

I conducted experiments across various learning rates (η=0.001 to 0.5). The results demonstrated that while higher learning rates can speed up training, they require careful monitoring of the Cross-Entropy loss to avoid "exploding" gradients.

**Batch Size Dynamics**

Small Batches (B=1,10): Provided high-frequency updates but exhibited "noisy" convergence.

Large Batches (B=100,1000): Utilized vectorization for computational efficiency and smoother optimization paths.

**Tech Stack**

**Language:** Python
**Optimization**: NumPy (Vectorized Matrix Calculus)
**Visualization**: Matplotlib
**Framework Benchmarking**: PyTorch & Torchvision

**Final Performance**

Successfully achieved consistent high accuracy (~84%+) on the 10-class MNIST classification task.



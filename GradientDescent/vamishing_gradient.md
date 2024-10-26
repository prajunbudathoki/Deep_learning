# Vanishing Gradient Problem in Neural Networks

## Overview
The **vanishing gradient problem** is a common issue in training deep neural networks, where the gradients of the loss function become very small as they backpropagate through the network layers. This reduces the ability of the model to learn and improve, especially in deeper layers.

## What Causes It?
The problem usually occurs when:
- **Deep networks**: Many layers in the model can make the gradient decrease significantly as it moves backward.
- **Activation functions**: Functions like sigmoid or tanh, which squash values between certain ranges, can reduce the gradient further.

## Why It Matters
When gradients are small:
1. The network learns very slowly.
2. Some layers, particularly those near the start, hardly improve.
3. The model may stop learning entirely if the gradients vanish completely.

## Solutions
1. **ReLU Activation Function**: Using Rectified Linear Unit (ReLU) helps maintain larger gradients.
2. **Batch Normalization**: It normalizes layer inputs, helping stabilize gradients.
3. **Skip Connections (Residual Networks)**: These provide alternate paths for gradient flow, improving learning.



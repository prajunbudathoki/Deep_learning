# Batch Normalization in Deep Learning

Batch normalization is a method used to stabilize and speed up the training of neural networks. It helps by normalizing the inputs for each layer so they have a similar distribution, leading to more stable and faster training.
    
## Why Use Batch Normalization?
- **Internal Covariate Shift**: Without normalization, each layer’s input distribution changes during training, which slows down learning.
- **Solution**: Batch normalization fixes this by keeping inputs to each layer in a stable range.

## How It Works
1. For each batch, calculate the mean and variance.
2. Normalize the inputs so they have a mean of 0 and a variance of 1.
3. Apply learnable scaling (gamma) and shifting (beta) to allow the network to learn optimal feature representations.

## Benefits of Batch Normalization
- **Faster Convergence**: Training becomes faster as input distribution is stabilized.
- **Allows Higher Learning Rates**: The network can be trained with higher learning rates safely.
- **Reduces Overfitting**: Acts as a regularizer, making the model generalize better.

Batch normalization is widely used in deep learning models, especially in convolutional and fully-connected networks, to make training efficient and stable.

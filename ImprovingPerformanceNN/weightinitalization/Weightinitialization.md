# Weight Initialization in Deep Learning

Weight Initialization is the process of setting the starting values of weights in a neural network before training. The choice of these values can have a significant impact on how effectively and efficiently the network learns.

## Why is Weight Initialization Important?
1. **Prevents Neurons from Getting Stuck**: Helps avoid inactive neurons that don’t contribute to learning.
2. **Speeds Up Learning**: Allows the model to converge faster by avoiding issues like exploding or vanishing gradients.
3. **Improves Accuracy**: Good initial weights lead to better performance by providing a good starting point.

## Types of Weight Initialization
1. **Zero Initialization**: Sets weights to zero (rarely used due to symmetry issues).
2. **Random Initialization**: Initializes weights randomly with small values, but can still cause exploding/vanishing gradients.
3. **Xavier (Glorot) Initialization**: Used with sigmoid or tanh activations to balance layer outputs.
4. **He Initialization**: Designed for ReLU activations to avoid the vanishing gradient problem.







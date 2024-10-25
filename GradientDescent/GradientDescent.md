# Gradient Descent in Neural Networks

## What is Gradient Descent?

Gradient Descent is an optimization algorithm used in neural networks to minimize the error or loss between predicted and actual outputs. The goal is to adjust the network's weights and biases to improve predictions.

### Key Concepts:

- **Loss Function:** Measures how far the network's predictions are from the actual target values.
- **Gradient:** Tells us the slope of the loss function with respect to the weights. It helps determine the direction in which the weights should be updated.
- **Descent:** Means we are going to move in the opposite direction of the gradient, which reduces the loss.

### How Gradient Descent Works:

1. **Initialization:** We start with random weights and biases.
2. **Forward Pass:** The neural network makes predictions based on current weights.
3. **Loss Calculation:** The difference between the predicted and actual values is calculated using a loss function.
4. **Backpropagation:** The gradient (derivative) of the loss with respect to each weight is calculated.
5. **Weight Update:** We adjust the weights using the formula:

   \[
   W_{\text{new}} = W_{\text{old}} - \eta \times \nabla L(W)
   \]
   where:
   - \( W_{\text{new}} \) is the updated weight.
   - \( W_{\text{old}} \) is the current weight.
   - \( \eta \) is the learning rate (step size).
   - \( \nabla L(W) \) is the gradient of the loss with respect to the weight.

6. **Iteration:** Steps 2 to 5 are repeated until the loss reaches a minimum.

### Learning Rate:

The **learning rate** controls how big each step is during the descent. A small learning rate means slow progress, while a large learning rate might overshoot the minimum.

### Summary:

- Gradient Descent helps the network learn by adjusting weights to minimize the error.
- It involves calculating the gradient (slope) of the loss function and updating weights in the opposite direction to reduce the loss.
- The process continues until the model reaches an optimal set of weights that minimizes the error.


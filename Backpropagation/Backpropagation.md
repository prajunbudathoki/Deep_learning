
# Backpropagation - A Simple Explanation

Backpropagation is an algorithm used in training neural networks. It adjusts the weights of the network to minimize the error (or loss) between the predicted output and the actual output.

## Steps of Backpropagation:

1. **Forward Pass**:
   The input data is passed through the neural network, and the output is generated. The output is compared with the true label, and the loss is calculated.

2. **Backward Pass (Error Propagation)**:
   The error is propagated back through the network. The goal is to compute the gradient of the loss function with respect to each weight, which tells us how to adjust the weights to minimize the loss.

3. **Weight Update**:
   Once we have the gradient, the weights are updated using the formula:
   \[
   w^{(new)} = w^{(old)} - \eta rac{\partial L}{\partial w}
   \]
   where:
   - \( w^{(new)} \) is the new weight,
   - \( w^{(old)} \) is the old weight,
   - \( \eta \) is the learning rate,
   - \( rac{\partial L}{\partial w} \) is the gradient of the loss function with respect to the weight.

## Formula Breakdown:
Let's take a simple neural network with one output neuron. Suppose:
- \( z = wx + b \), where \( w \) is the weight, \( x \) is the input, and \( b \) is the bias.
- The activation function \( a = \sigma(z) \), where \( \sigma \) is a non-linear function like the sigmoid.

The **loss function** \( L \) is the difference between the predicted output \( a \) and the true output \( y \). For example, with Mean Squared Error (MSE) loss:
\[
L = rac{1}{2}(a - y)^2
\]

### Backpropagation steps:

1. **Calculate the gradient of the loss w.r.t the output**:
   \[
   rac{\partial L}{\partial a} = a - y
   \]

2. **Calculate the gradient of the output w.r.t. the weighted sum**:
   \[
   rac{\partial a}{\partial z} = \sigma'(z)
   \]
   where \( \sigma'(z) \) is the derivative of the activation function.

3. **Gradient of the loss w.r.t. \( z \)**:
   \[
   rac{\partial L}{\partial z} = rac{\partial L}{\partial a} \cdot rac{\partial a}{\partial z}
   \]

4. **Gradient of the loss w.r.t the weight \( w \)**:
   \[
   rac{\partial L}{\partial w} = rac{\partial L}{\partial z} \cdot rac{\partial z}{\partial w} = rac{\partial L}{\partial z} \cdot x
   \]

5. **Weight update**:
   \[
   w^{(new)} = w^{(old)} - \eta \cdot rac{\partial L}{\partial w}
   \]

By repeating these steps for all layers, the network's weights are adjusted to minimize the error.

## Summary:

Backpropagation uses the chain rule of calculus to calculate the gradient of the loss function with respect to each weight. The weights are then updated using these gradients to reduce the loss and improve the network's performance.

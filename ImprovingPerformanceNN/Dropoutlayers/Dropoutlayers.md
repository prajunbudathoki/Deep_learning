# Dropout Layers in Neural Networks

Dropout is a technique used in neural networks to help prevent overfitting. Overfitting happens when a model learns the training data too well, making it perform poorly on new data. Dropout randomly “drops out” or turns off some neurons (nodes) during training, helping the network learn more general patterns instead of memorizing the data.

## Why Use Dropout?
In each round of training (epoch), some neurons are randomly “dropped” so they don’t participate. This forces the network to use other neurons and connections, making it more robust. It’s like asking different groups of friends to solve a puzzle each time—each group learns the puzzle better by working together in new ways.

## How Dropout Works
1. **Set Dropout Rate**: Define a dropout rate, like 0.2 (20%), which represents the percentage of neurons to turn off.
2. **Apply During Training**: Randomly turn off neurons at each round of training. The model trains with fewer neurons each time.
3. **Use Full Network in Testing**: Once training is complete, all neurons are active again for final predictions, so the model can use everything it learned.

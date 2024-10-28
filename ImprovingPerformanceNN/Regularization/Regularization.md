# Regularization

Regularization is a technique used in machine learning/deep learning to prevent overfitting. Think of it as a way to “keep our model in check,” so it doesn’t get too focused on small details of the training data and can generalize better to new data.

## Why Use Regularization?
When a model learns too much, it picks up noise and tiny details that don't actually help it understand new data—this is overfitting. Regularization discourages the model from doing that by adding a penalty to the learning process, which makes it focus on the bigger picture.

## Common Types of Regularization
1. **L1 Regularization (Lasso)**: Adds a penalty equal to the absolute value of the magnitude of coefficients. It encourages simpler models with fewer parameters by driving some weights to zero, effectively “ignoring” certain features.

2. **L2 Regularization (Ridge)**: Adds a penalty equal to the square of the magnitude of coefficients. It doesn’t set weights to zero but makes them smaller, reducing their impact.

3. **Dropout**: Temporarily “drops out” (ignores) random neurons during training, forcing the network to not rely too heavily on specific paths.

4. **Early Stopping**: Stops training when the model starts overfitting (when it performs well on training data but worsens on validation data).

## Benefits of Regularization
Regularization helps create a more robust, general model that works well with new data by avoiding overfitting. It’s like a gentle reminder to “focus on the main features, not the little quirks.”




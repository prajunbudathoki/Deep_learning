# Exponentially Weighted Moving Average (EWMA)

## Overview

Exponentially Weighted Moving Average (EWMA) is a statistical technique for smoothing data, especially useful for analyzing noisy signals or tracking trends over time. It assigns exponentially decreasing weights to older observations.

### Formula

\[
EWMA_t = \alpha \cdot x_t + (1 - \alpha) \cdot EWMA_{t-1}
\]

Where:
- \( \alpha \): Smoothing factor (0 < \( \alpha \) ≤ 1)
- \( x_t \): Current observation
- \( EWMA_{t-1} \): Previous EWMA value

### Characteristics
- Reduces noise while retaining the signal's trend.
- More responsive to recent changes than a simple moving average.

---

## Applications in Deep Learning

1. **Gradient Smoothing**  
   EWMA is integral to optimization algorithms like **Adam** and **RMSprop**, ensuring stable updates by maintaining moving averages of gradients.

2. **Loss Monitoring**  
   Smoothing training loss curves to identify trends and detect anomalies.

3. **Learning Rate Adjustment**  
   Helps in scheduling dynamic learning rates by observing smoothed metrics.

4. **Anomaly Detection**  
   Applied in time-series forecasting to detect outliers based on deviations from smoothed trends.

5. **Data Preprocessing**  
   Smooths noisy input data to improve model performance.



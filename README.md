# Machine-Learning-Basics
Implementations of machine learning algorithms from scratch.

## Algorithms implemented:
- **Linear Regression:**
Supervised learning algorithm used for computing parameters (theta) such that the predicted linear model is a line of best fit for the given input features (X_train) and output (y_train).
  - **Linear Regression using Batch Gradient Descent:**
  All the training samples are taken into consideration while computing the gradient.
  - **Linear Regression using Stochastic Gradient Descent:**
  The gradient is computed using a single training sample.
  **NOTE:** BGD takes steps directly towards the minima of the cost function (which is a convex function of theta), while SGD moves towards the minima in a noisy manner and does not converge exactly to the global minima (but attains a value fairly close to it). However, SGD is faster than BGD and is thus used while training the model using a large number of training samples.
  
- **K-Nearest Neighbours:**
Supervised learning algorithm used for classification.

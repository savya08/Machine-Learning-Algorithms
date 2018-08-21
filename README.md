# Machine-Learning-Basics
Implementations of machine learning algorithms from scratch.

## Algorithms implemented:
- **Linear Regression:**
Supervised learning algorithm used for computing parameters (theta) such that the predicted linear model is a line of best fit for the given input features (X_train) and output (y_train).
  - **Linear Regression using Batch Gradient Descent:**
  All the training samples are taken into consideration while computing the gradient.
  - **Linear Regression using Stochastic Gradient Descent:**
  The gradient is computed using a single training sample.
  BGD takes steps directly towards the minima of the cost function (which is a convex function of theta), while SGD moves         towards the minima in a noisy manner and does not converge exactly to the global minima (but attains a value fairly close to   it). However, SGD is faster than BGD and is thus used while training the model using a large number of training samples.
  - **Linear Regression using Normal Equation:**
  It is a non-iterative algorithm used for directly finding the theta vector which minimises the cost function.
  Formula used: theta = (X<sup>T</sup>X)<sup>-1</sup>X<sup>T</sup>y
  
- **Logistic Regression:**
Supervised learning algorithm used for classifying data into binary calsses such as 0/1, True/False, Yes/No. In this algorithm, parameters are computed for a desicion boundary that saperates the two classes in the best possible manner.
  
- **K-Nearest Neighbours:**
Supervised learning algorithm used for classification of data into a number of classes. A given test point is classified on the basis of the classes of k training points nearest to it.

- **K-Means Clustering:**
Unsupervised learning algorithm used for clustering data. The idea is to iteratively find k centroids for k clusters on the basis of the (unlabeled) training data available. Testing points are classified on the basis of their distance from the centroids - a point belongs to the cluster having its centroid nearest to it.

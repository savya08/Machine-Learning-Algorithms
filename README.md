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
  - **Linear Regressioin using Mini-Batch Gradient Descent:**
  The gradient is computed using a mini-batch of examples and the update is made to reduce the cost for the considered mini-batch. If batch size is equal to 1, it is called stochastic gradient descent. Similarly, if batch size is m (the number of training examples), it becomes batch gradient descent.
  - **Linear Regression using Normal Equation:**
  It is a non-iterative algorithm used for directly finding the theta vector which minimises the cost function.\
  Formula used: theta = (X<sup>T</sup>X)<sup>-1</sup>X<sup>T</sup>y
  - **Locally Weighted Linear Regression:**
  A regression technique used to make predictions on non-linear data. It can be implimented using gradient descent algorithm or       using a closed form solution.\
  Formula used (Gradient Descent): theta = theta - learning_rate * weight * gradient\
  Formula used (Closed Form): theta = (X<sup>T</sup>WX)<sup>-1</sup>X<sup>T</sup>Wy
  
- **Logistic Regression:**
Supervised learning algorithm used for classifying data into binary calsses such as 0/1, True/False, Yes/No. In this algorithm, parameters are computed for a desicion boundary that saperates the two classes in the best possible manner.
  
- **K-Nearest Neighbours:**
Supervised learning algorithm used for classification of data into a number of classes. A given test point is classified on the basis of the classes of k training points nearest to it.

- **K-Means Clustering:**
Unsupervised learning algorithm used for clustering data. The idea is to iteratively find k centroids for k clusters on the basis of the (unlabeled) training data available. Testing points are classified on the basis of their distance from the centroids - a point belongs to the cluster having its centroid nearest to it.

- **Naive Bayes Classifiers:**
It is a supervised learning algorithm which uses Bayes theorem to calculate the maximum posterior probability (probability of an output given some info as input - here, the probability of whether the person plays or not on a given day given the values of the attributes for the day) and thus make predictions. It assumes complete independence between the attributes - disavantage. It is quick in making predictions as no iterative parameter optimisation is needed - advantage.

- **Support Vector Machines**
A Support Vector Machine (SVM) is a discriminative classifier formally defined by a separating hyperplane. In other words, given labeled training data (supervised learning), the algorithm outputs an optimal hyperplane which categorizes new examples. In two dimentional space this hyperplane is a line dividing a plane in two parts where in each class lay in either side.

- **Neural Network:**
Artificial neural networks are one of the main tools used in machine learning. As the “neural” part of their name suggests, they are brain-inspired systems which are intended to replicate the way that we humans learn. Neural networks consist of input and output layers, as well as (in most cases) a hidden layer consisting of units that transform the input into something that the output layer can use. They are excellent tools for finding patterns which are far too complex or numerous for a human programmer to extract and teach the machine to recognize.

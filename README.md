# Support Vector Machine on make_moons Dataset

## Overview
This project focuses on implementing a Support Vector Machine (SVM) for a two-class classification task using the non-linear `make_moons` dataset from the scikit-learn library. The goal is to experiment with different kernel functions and tune their respective hyperparameters for optimal performance.

## Dataset

The `make_moons` dataset is a synthetic dataset that generates two interleaving half circles. It is a common dataset used to test the performance of classification algorithms, particularly for non-linear problems.

- **Number of samples:** 500
- **Noise level:** Configurable as per user preference

## Kernels Explored

We will implement SVMs using the following kernels:

1. **Linear Kernel**
2. **Radial Basis Function (RBF) Kernel**
3. **Polynomial Kernel (Degree 3)**
4. **Sigmoid Kernel**

## Hyperparameter Tuning

For each kernel, we utilize the `RandomizedSearchCV` class from the scikit-learn library to tune the hyperparameters. The best set of hyperparameters for each kernel will be reported.

## Visualization

The provided `plt_moons()` function is used to plot the decision boundaries of the trained SVM models on the training data.

## Results

The best hyperparameters for each kernel will be outputted in the console. The decision boundary plots will also be displayed for each kernel.

## Evaluation

The models will be evaluated based on their classification accuracy on the test set and the quality of their decision boundaries.

# Support Vector Regression on Diabetes Dataset

## Overview

This project implements Support Vector Regression (SVR) for predicting a regression function using the diabetes dataset provided by the scikit-learn library. The dataset includes 10 numerical features derived from 442 diabetic patients and one numerical output feature.

## Dataset

- **Features:** 10 numerical features, with values ranging from approximately -0.2 to 0.2.
- **Target:** One numerical output, with values ranging from -25 to -346.

The goal is to predict the target variable using the features provided.

## Kernels Explored

We will implement SVR using the following kernels:

1. **Linear Kernel**
2. **Radial Basis Function (RBF) Kernel**
3. **Polynomial Kernel**

## Hyperparameter Tuning

For each kernel, we use the `GridSearchCV` class from the scikit-learn library to fine-tune the hyperparameters. The best set of hyperparameters for each kernel will be reported.

## Linear Regression Baseline

We will use the `LinearRegression` class from scikit-learn to establish a baseline by finding the linear regression's true value on the test data.

## Evaluation

For each kernel's best hyperparameters, we will report:

- **Accuracy**
- **Root Mean Square Error (RMSE)**

These metrics will help us evaluate the model's performance.

## Results

The best hyperparameters for each kernel will be outputted in the console. Accuracy and RMSE values for each kernel will also be reported.

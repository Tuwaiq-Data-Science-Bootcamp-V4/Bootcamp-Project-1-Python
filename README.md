# Linear Regression in Python

This project implements a simple Linear Regression algorithm in Python. It consists of several functions that allow you to perform linear regression, calculate the cost, gradients, and optimize the coefficients to fit the data. Using Mean Squared Error and Gradient descent, it was able to perform in the right direction.

## Functions

### 1. `cost_function(x, y, w, b)`

This function takes input variables `x` and output variables `y`, along with coefficients `w` and `b`, and calculates the cost using the Mean Squared Error (MSE) formula. It returns the computed cost.

### 2. `gradient(x, y, w, b)`

The `gradient` function takes input variables `x` and output variables `y`, as well as coefficients `w` and `b`. It calculates the gradients required to update the coefficients `w` and `b` during the training process. The function returns the computed gradients.

### 3. `fit(X, y, w_in, b_in, cost_function, gradient_function, alpha, num_iters)`

The `fit` function is responsible for training the linear regression model. It takes input data `X`, output data `y`, initial coefficients `w_in` and `b_in`, the `cost_function`, `gradient_function`, learning rate `alpha`, and the number of iterations `num_iters`.

During training, the function iteratively updates the coefficients `w` and `b` using the provided `cost_function` and `gradient_function`, to hopefully minimize the cost function. It returns the optimal coefficients after training.

## Usage

Here's an example of how you can use these functions to perform linear regression:

```python
# Define your input data X and target data y

# Set initial coefficients w and b, you can use eaither zeros or random values

# Set the learning rate alpha and the number of iterations

# Train the model and get the optimal coefficients
optimal_w, optimal_b = fit(X, y, w_in, b_in, cost_function, gradient_function, alpha, num_iters)

# Now you can use the optimal_w and optimal_b to make predictions.
```

## The Linear Regression line with the actual data

![Image](https://github.com/Khalid-Ibrahim1/Bootcamp-Project-1-Python/blob/main/performance.png)

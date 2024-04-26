# Gradient Descent

## Introduction

[Gradient descent](https://en.wikipedia.org/wiki/Gradient_descent) is a fundamental optimization algorithm used in machine learning to minimize a function. It is particularly effective for finding the minimum of a cost function in various types of models, including linear regression, logistic regression, and neutral networks. The main idea behind Gradient Descent is to iteratively adjust the parameters of a model to minimize the cost function. **The algorithm uses the gradient (or slope) of the cost function to determine the direction in which the function has the steepest descent and updates the parameters in the opposite direction to reach the minimum value.**

---

## Algorithm

The algorithm works as follows:

<p align="center">
    <img src="gradient_descent.png">
</p>

1. **Initialization:** Start with random values for the parameters (weights and biases in the context of neural networks)

2. **Compute Gradient:** Calculate the gradient of the cost function with respect to each parameter. The gradient is a vector of partial derivatives, where each element is the derivative of the cost function relative to one parameter

3. **Update Parameters:** Adjust the parameters in the direction that reduces the cost function. This is done by substracting a faction of the gradient from the current parameters: $a_{n+1} = a_n - \gamma f'(a_n)$. Here, $a_n$ represents the parameters, $\gamma$ is the learning rate (a small positive number determining the size of the step), and $f'(a_n)$ is the gradient of the cost function

4. **Iterate:** Repeat the process (compute gradient and update parameters) until the cost function converges to a minimum or a predefined number of iterations is reached

---

## Advantages and Disadvantages
Advantages:
- Gradient Descent is straightforward to understand and implement for optimizing various types of cost functions
- It can be used with almost any differentiable function, including complex neural networks

Disadvantages:
- In non-convex functions, Gradient Descent can get stuck in local minima or saddle points rather than finding the global minimum.
- Choosing the wrong learning rate can make the algorithm coverage too slowly or diverge

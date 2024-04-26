# Perceptron

## Introduction

The perceptron is a type of artificial neuron used in machine learning, representing the simplest form of a neural network. It's essentially a model of a single neuron, which serves as the foundational building block for more complex neural work architectures.

---

## Algorithm

<p align="center">
    <img src="Perceptron.png">
</p>

The algorithm works as follows.

1. **Inputs and Weights:** The perceptron receives inputs, each of which is associated with a weight

2. **Summation and Activation:** The perceptron multiplies each input by its corresponding weight and sums these products. Often, a bias term is also added to the sum to help the model adjust its output. The resulting total is then passed through an activation function. The most basic form of activation function used in a perceptron is a step function, which outputs either one value if the total sum is above a certain threshold or another value if it is below

3. **Output:** The output of perceptron is used for binary classification tasks. It either activates or doesn't, based on whether the input data belong to one category or another.

4. **Learning:** The perceptron adjusts its weights based on the errors it makes in predictions during training. This process is learning. The typical learning rule used is the perceptron learning rule, where the weights are updated to minimize the error in predictions.

---

## Advantages and Disadvantages
Advantages:
- The perceptron is simple to implement and understand, making it a good starting point for learning about neural networks
- It is computationally efficient because it involves straightforward matrix operations

Disadvantages:
- The perceptron can only classify data that are linearly separable. If the data cannot be separated by a single line, the perceptron will not be able to find a solution
- Unlike some other classifiers like logistic regression, perceptrons do not provide probability estimates for predictions, only hard thresholds
- A single perceptron can only handle binary classification tasks
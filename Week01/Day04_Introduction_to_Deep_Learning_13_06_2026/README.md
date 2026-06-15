# Day 04 - Introduction to Deep Learning

## Objective

The objective of this activity was to understand the fundamentals of Deep Learning and implement a Perceptron from scratch using Python.

A Perceptron is the simplest form of an Artificial Neural Network and serves as the foundation of modern Deep Learning models.

This implementation was performed without using any Machine Learning or Deep Learning libraries in order to understand the internal working of a neural network.

---

## Topics Covered

* Introduction to Deep Learning
* Evolution from Machine Learning to Deep Learning
* Perceptron
* Neural Networks
* Inputs, Weights and Bias
* Activation Functions
* Error Calculation
* Perceptron Learning Rule
* Weight Update Mechanism
* Backpropagation (Concept)
* Optimization Techniques

---

## Practical Implementation

### Perceptron for AND Gate

A Perceptron was implemented from scratch using pure Python and trained to learn the AND Gate logic.

The implementation included:

1. Initializing weights and bias
2. Defining training data
3. Computing weighted sums
4. Applying a Step Activation Function
5. Calculating prediction error
6. Updating weights and bias using the Perceptron Learning Rule
7. Testing the trained perceptron

---

## AND Gate Truth Table

| Input 1 | Input 2 | Output |
| ------- | ------- | ------ |
| 0       | 0       | 0      |
| 0       | 1       | 0      |
| 1       | 0       | 0      |
| 1       | 1       | 1      |

The perceptron was trained using this truth table.

---

## Activation Function

A Step Activation Function was used.

Output:

* 1 if z ≥ 0
* 0 if z < 0

---

## Results

After training for multiple epochs, the perceptron successfully learned the AND Gate logic.

Testing Results:

| Input | Predicted Output |
| ----- | ---------------- |
| [0,0] | 0                |
| [0,1] | 0                |
| [1,0] | 0                |
| [1,1] | 1                |

The predicted outputs matched the expected outputs, indicating successful learning.

---

## Learning Outcomes

After completing this activity, I learned:

* The difference between Machine Learning and Deep Learning.
* The structure and working of a Perceptron.
* The role of inputs, weights, and bias.
* The purpose of activation functions.
* How prediction errors are calculated.
* How weights and bias are updated during training.
* The concept of learning through multiple epochs.
* The foundation of Artificial Neural Networks and Deep Learning.

---

## Files Included

* Perceptron_From_Scratch_AND_Gate.ipynb
* Notes.md
* README.md

---

## Conclusion

This activity provided a practical introduction to Deep Learning through the implementation of a Perceptron from scratch. The perceptron was successfully trained to learn the AND Gate logic using the Perceptron Learning Rule. The experiment demonstrated how neural networks process inputs, generate predictions, calculate errors, and improve performance through weight updates. Understanding the perceptron forms the foundation for studying advanced Deep Learning architectures such as ANN, CNN, RNN, LSTM, and Transformers.
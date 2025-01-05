Perceptron and MultiPerceptron Implementation

Overview

This project implements the Perceptron algorithm for binary classification and extends it to the MultiPerceptron for multiclass classification. Written in Java, this project demonstrates the foundational principles of machine learning with easy-to-follow code and examples.


Features

🧠 Perceptron:

Binary Classification, Classifies inputs into two categories (1 or -1).

Adjustable Weights: Learns by adjusting weights based on misclassified inputs.

Simple and Lightweight: Suitable for linear classification tasks.

🔗 MultiPerceptron

Multiclass Classification: Handles multiple classes using a "one-vs-all" approach.

Modular Design: Built using multiple single-layer perceptrons.

Flexible: Can predict the class with the highest confidence.


Technologies Used

Java: Object-oriented programming language.

Core Programming Concepts: Classes, methods, loops, and arrays.


How It Works

Perceptron

Initialization: Define the number of inputs and initialize the weights.

Training: Update weights if the predicted output differs from the expected output.

Prediction: Compute the weighted sum of inputs and classify as 1 or -1.

MultiPerceptron

Initialization: Create multiple Perceptrons (one for each class).

Training: Train each Perceptron to recognize its class versus all others.

Prediction: Select the class with the highest weighted sum.

#Perceptron and MultiPerceptron Implementation
Overview
This project implements the Perceptron algorithm for binary classification and extends it to the Multi-layer Perceptron (MultiPerceptron) for multiclass classification. The implementation is written in Java and demonstrates how these fundamental machine learning models function by training and predicting on example data.

Features
Perceptron
Single-layer perceptron designed for binary classification.
Utilizes a simple training mechanism to adjust weights based on prediction errors.
Includes a prediction method to classify data into two categories (1 or -1).
MultiPerceptron
Extends the Perceptron to handle multiclass classification problems.
Uses multiple perceptrons, each representing one class, and predicts the class with the highest weighted sum.
Trains each perceptron using a one-vs-all approach.
Technologies Used
Java
Core Java concepts like classes, object-oriented programming, and arrays are used to build the implementation.
How It Works
Perceptron
Initialization:
Takes the number of inputs (n) and initializes the weight array.
Training:
Adjusts weights based on the difference between the predicted and actual labels.
Prediction:
Uses the weighted sum of inputs to classify as 1 (positive) or -1 (negative).
MultiPerceptron
Initialization:
Creates m Perceptrons, one for each class, where m is the number of classes.
Training:
Trains each Perceptron to classify its corresponding class against all other classes.
Prediction:
Compares the outputs of all Perceptrons and selects the class with the highest weighted sum.
Usage
Perceptron Example:
java
Perceptron perceptron = new Perceptron(3);  
double[] training1 = { 5.0, -4.0, 3.0 };  
double[] training2 = { 2.0, 3.0, -2.0 };  
perceptron.train(training1, 1);  
perceptron.train(training2, -1);  
System.out.println(perceptron);  
MultiPerceptron Example:
java
MultiPerceptron multiPerceptron = new MultiPerceptron(2, 3);  
double[] training1 = { 5.0, -4.0, 3.0 };  
double[] training2 = { 2.0, 3.0, -2.0 };  
multiPerceptron.trainMulti(training1, 1);  
multiPerceptron.trainMulti(training2, 0);  
System.out.println(multiPerceptron);  
Project Structure
bash
/src  
├── Perceptron.java          # Single-layer perceptron implementation  
├── MultiPerceptron.java     # Multi-layer perceptron implementation  
└── README.md                # Project documentation  
Learning Outcomes
Understand the fundamentals of Perceptron and MultiPerceptron algorithms.
Learn how to implement machine learning models in Java.
Gain insights into binary and multiclass classification processes.
Future Enhancements
Add support for non-linear problems using activation functions.
Implement learning rate adjustments for more efficient training.
Explore visualization tools for decision boundaries.
Contributions
Feel free to fork this repository, submit issues, or suggest improvements through pull requests. Contributions are always welcome!

License
This project is licensed under the MIT License.

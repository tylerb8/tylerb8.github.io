---
layout: project
type: project
image: images/iris-dataset.png
title: Iris Dataset
permalink: projects/iris
date: 2021-07-11
labels:
  - Python
  - Jupyter Notebook
summary: Single Neuron Networks: Iris DataSet
---


## Introduction
Neural Networks, are computational algorithms or models designed as per the structure of the human brain.  
In the Perceptron notebook we learned how to build simple neural networks "one-neuron networks". Where for each neuron, we trained the neuron (ie set the weights) by minimizing a different kind of loss function for each model. We built each neuron with the help of keras, and gradient descent to learn the weight.

### The three basic models we learned in class with their loss function:

 - Perceptron: activation is linear, train by minimizing the ramp loss = max(0, -y_true* y_predicted)  
 - The Linear Regression classifier (Fisher Discriminant): activation is linear, train by minimizing square loss (y_true - y_predicted)^2  
 - Support vector machine: activation is linear (for now). We train by minimizing the hinge loss = max(0, 1- y_true* y_predicted), but to the hinge loss, we add a (1/C)||w||^2 term, where C is some constant. In machine learning parlance, adding a ||w||^2 term to the loss is called l2 regularization. So this is a single neuron, linear activation, trained using hinge loss with l2 regularization.

## Iris dataset

In this lab we used the Iris dataset which contains 3 classes with 50 instances each, where each class refers to a type of iris plant. One class is linearly separable from the other 2; the latter is not linearly separable from the others. We will be using each model to demonstrate how they can be used to linearly separate the two linearly separable classes.

The two linearly Separable classes are sepal width (feature 1) and petal length (feature 2)

    
<img class="ui medium right floated rounded image" src="../iris1.png">




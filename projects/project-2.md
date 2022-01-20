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
  - Keras
  - Classification
summary: Single Neuron Networks - Iris Dataset
---


<img class="ui large centered image" src="../images/iris-dataset.png">

## Welcome
Neural Networks, are computational algorithms or models designed as per the structure of the human brain. In the Perceptron notebook we learned how to build simple neural networks "one-neuron networks". Where for each neuron, we trained the neuron (ie set the weights) by minimizing a different kind of loss function for each model. We built each neuron with the help of keras, and gradient descent to learn the weight.


## Iris dataset

In this lab we used the Iris dataset which contains 3 classes with 50 instances each, where each class refers to a type of iris plant. One class is linearly separable from the other 2; the latter is not linearly separable from the others. We will be using each model to demonstrate how they can be used to linearly separate the two linearly separable classes.

### The two linearly Separable classes are sepal width (feature 1) and petal length (feature 2)

```
# What the Iris dataset looks like plotted 
    
from sklearn import datasets iris = datasets.load_iris() print(dir(iris))
import matplotlib.pyplot as plt from mpl_toolkits import mplot3d
    

fig = plt.figure()  
display(fig)  
ax = plt.axes(projection='3d')  
figiris = ax.scatter(iris.data[:,0],iris.data[:,1],iris.data[:,2],c=iris.target) 
ax.set_xlabel(iris.feature_names[1]+' (1)') 
ax.set_ylabel(iris.feature_names[2]+' (2)') 
ax.set_zlabel(iris.feature_names[0]+' (0))')
	
# this adjusts the space around the plot so we can read the z label 
plt.gcf().subplots_adjust(left=-0.5,bottom=-0.3)

plt.colorbar(figiris) 
ax.view_init(45,45)
```
    


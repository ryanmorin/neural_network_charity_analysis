# Neural Network Charity Analysis

## Project Overview

The project uses the data of over 34,000 organizations to create a binary classification neural network model. The project's goal, with 75% accuracy, is to create a model capable of predicting whether organizations will be financially successful. The model uses the TensorFlow module of Python to create a training and testing group.  Ultimately the model achieved a success rate of roughly 73%.  Further improvements: such as additional nodes, layers or epochs could be insituted that could improve the model's accuracy.

## Technology

* TensorFlow 2.8.0
* Python 3.7.11

## Results

Model improvements increased the accuracy of the model from 72% to roughly 73% and lowered the loss from 57% to 55%. The following are some of the project highlights:

1. Target variable - The target variable is the varaible that we're trying to predict. In this case we're interested in the 'IS_SUCCESSFUL' varaible.
2. Feature variables - Changes in the feature variables influence the value of the target variable (feature variables are independent variables). In this case the first part of the project had 43 variables. In part 3 of the project I reduced the number of varaibles to 39 in an attempt to improve the models accuracy.
3. Some varaibles - such as Name or EIN are neither target nor feature variables. These variables simply describe data but are not expected to influence the Target variable's value.
4. Originally I chose 2 hidden layers.  8 nodes in the first hidden layer and 5 in the second hidden layer. I decided to take a trial and error approach to the problem so I randomly choose the number of layers and nodes to see how the model performed.   
5. I wasn't able to achieve the target performance.  After the 3 attempts I was able to achieve roughly 73% accuracy. Further improvements such as additional nodes, layers or epochs could improve the overall accuracy.
6. I took the following action to improve the model's performance:
   * I added additional Layers to the model
   * I increased the number of nodes in each of the layers
   * I deleted fields that I felt had little impact on the overall models predictability.

## Summary

The model achieved overall accuracy of roughly 72%.  After tweaks were made to the number of nodes, the number of layers and the number of feature variables, the model's overall accuracy increased marginally. I could've tried adding more of the same (more nodes, more layers etc) to see if the performance improved. Conversely I could've choosen to approach the problem differently and used a type of model to achieve the same result. A random forest classifier (RFC) consists of a large number of individual decision trees that operate as an ensemble. Each individual tree in the random forest spits out a class prediction and the class with the most votes becomes our model’s prediction. Fequently RFC models require fewer computational resources compared to a neural network model. The main benefit of a model like RFC, is that it is able to provide more insight into how individual variables contribute to the model's results.  This benefit would be helpful explaining the models results to others.

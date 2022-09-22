# MIT-introductiontodeeplearning

This repo contains all of the labs completed as a part of MIT 6.S191 Introduction to Deep Learning.

## Lab 1. Deep Sequence Modeling

### Part 1: TensorFlow

This lab outlines the general workflows as well as the underlying math associated with building, training and 
evaluating models using TensorFlow and Keras. 

### Part 2: Music Generation

In this lab a recurrent neural network was built and trained on 817 irish folk songs represented in the ABC notation. 
A batch training method was used to train the model to predict the 'next character' of a given series, given as input.
Following hyperparameter tuning, the model was reconfigured to generate a new irish folk song from scratch, which can
be played at the end of the notebook.


## Lab 2. Deep Computer Vision and Deep Generative Modeling

### Part 1: MNIST

In this lab the famous MNIST dataset was approached using three different ML techniques. First, a standard single hidden 
layer, densely connected NN was built and trained to a test accuracy of ~96.5%. Then a convolutional neural network (CNN) 
consisting of multiple layers on convolution together with max-pooling was built and trained to a test accuracy of 
~99.0%. Finally, this same CNN model architecture was trained again, this time using a lower level tf.GradientTape 
approach, to a test accuracy of ~98.3.

### Part 2: Debiasing

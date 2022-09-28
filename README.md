# [MIT 6.S191 Introduction to Deep Learning](http://introtodeeplearning.com/)

This repo contains all of the labs completed as a part of MIT's 6.S191 Introduction to Deep Learning course.

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
consisting of multiple layers of convolution together with max-pooling was built and trained to a test accuracy of 
~99.0%. Finally, this same CNN model architecture was trained again, this time using a lower level tf.GradientTape 
approach, to a test accuracy of ~98.3.

### Part 2: Debiasing (DB-VAE)

This lab explores the concept of debiasing, following the approach outlined in Uncovering and [Mitigating Algorithmic 
Bias Through Learned Latent Structure (Amini, 2019).](http://introtodeeplearning.com/AAAI_MitigatingAlgorithmicBias.pdf)

First, two datasets, a set of face images and a set of images that are not faces, are used to train a facial detection 
model. This model is then evaluated using a third, seperate, test dataset containing face images with equal representation 
across all combinations of two demographics / features of interest: skintone and gender. Test accuracy varied widely across 
the 4 demographic categories present in the test dataset, ranging from ~40% to ~75%.

Then, with the goal of mitigating potential biases learned from the two training datasets, a debiasing variational 
autoencoder (DB-VAE) is trained and evaluated using the same 3 datasets as before. The DB-VAE learns the latent variables 
of the training set faces and then uses them to adaptively re-sample the set. This increases the chance of under-represented
faces being sampled and vice versa for over-represented faces.

In the end, the DB-VAE is succesful in debaising the model, as previously "innacurate" demographics are much more accurate 
and accuracies are more closely spread (~63% to 74%).

## Lab 3

### Reinforcement Learning


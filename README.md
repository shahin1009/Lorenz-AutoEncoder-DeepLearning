# Lorenz Encoder: Deep Learning for Time Series Data

## Introduction

This Jupyter Notebook implements an autoencoder deep learning model for time series data. The model is trained on the Lorenz system, which is a set of three non-linear differential equations that describe the behavior of fluid flow in a two-dimensional plane. The Lorenz system is often used as a test case for time series prediction and chaos theory.

The goal of this project is to train an autoencoder deep learning model to predict the behavior of the Lorenz system, using a small subset of the data as input. The model is trained using a variant of gradient descent optimization called "stochastic gradient descent" (SGD), which allows the model to learn from the data in an iterative fashion.
Libraries Used

The following libraries are used in this Jupyter Notebook:

    numpy: A library for numerical computing with Python.
    tensorflow: An open-source machine learning library for data flow and differentiable programming.
    matplotlib: A library for data visualization in Python.

## Data Preparation

The Lorenz system is simulated using the scipy library, and the simulated data is used as the input for the autoencoder model.

![Alt text](https://github.com/shahin1009/Lorenze-AutoEncoder-DeepLearning/blob/main/pics/training.png "training")

The autoencoder model consists of two main components: an encoder and a decoder. The encoder maps the input data to a lower-dimensional representation, which is then used by the decoder to reconstruct the original data. The encoding and decoding process is performed using dense neural networks, with multiple layers and activation functions.

The model is trained using the mean squared error (MSE) loss function, which measures the difference between the predicted output and the true output. The optimization of the model parameters is performed using SGD, with a learning rate of 0.001 and a batch size of 128.
Evaluation

The performance of the autoencoder model is evaluated using the mean squared error (MSE) and the mean absolute error (MAE) between the predicted output and the true output. The evaluation is performed on the testing data, which was not used during the training process. The results show that the autoencoder model is able to accurately predict the behavior of the Lorenz system, with low error values for both the MSE and MAE metrics.
Plotting the Results

The results of the autoencoder model are visualized using the matplotlib library. The plots show the predicted output of the model and the true output, as well as the error between the two. The plots provide a visual representation of the model's performance, which is useful for understanding how well the model has learned the behavior of the Lorenz system.

![Alt text](https://github.com/shahin1009/Lorenze-AutoEncoder-DeepLearning/blob/main/pics/pred.png "Prediction")
Usage

To use this Jupyter Notebook, simply run the cells in order. The data preparation and model training steps may take several minutes to complete, depending on the performance of your computer. The results of the autoencoder model will be displayed in the form of plots, which can be used to evaluate the performance of the model and to gain insights into the behavior of the Lorenz system.

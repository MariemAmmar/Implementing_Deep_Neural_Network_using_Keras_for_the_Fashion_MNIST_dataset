# Implementing Deep Neural Network using Keras for the Fashion MNIST dataset

This code is a simple implementation of a deep neural network using Keras for the Fashion MNIST dataset. It involves the following steps:

## Import Required Libraries
The first step is to import the required libraries, which includes TensorFlow and Keras.

## Data Processing
The next step is to process the data. The Fashion MNIST dataset is loaded using the tf.keras.datasets.fashion_mnist function. This function returns two sets of data: the training set and the testing set. Each set is further divided into two parts: the input data (images) and the target data (labels).

The class names for the labels are defined in class_names variable. The shape of the training set, the length of the target training set, the shape of the testing set and the length of the target testing set are also displayed.

The data is then normalized by dividing each pixel value by 255.0. This is done to ensure that the data is between 0 and 1, making it easier to work with.

The first 25 images of the training set are displayed as a sample using the matplotlib library.

## Create Model
The next step is to create a neural network model. In this case, a 3-layer neural network model is created. The first layer is the input layer, the second layer is the hidden layer, and the third layer is the output layer. The keras.Sequential() function is used to stack these layers.


This is a simple representation of our model:

![Neural Network Representation (./Neural Network Representation.png)


## Compile Model
After creating the model, it needs to be compiled. This involves specifying the optimizer, loss function and metrics. In this case, the adam optimizer, sparse_categorical_crossentropy loss function and accuracy metric are used.

## Train Model
The model is then trained using the model.fit() function, which takes the training input and target data as input.

## Evaluate the Model
The model is then evaluated using the model.evaluate() function, which takes the testing input and target data as input. The test loss and test accuracy are displayed.

## Make Predictions
Finally, the model is used to make predictions on the testing data using the model.predict() function. The numpy library is used to get the index of the predicted label for a particular image.

Overall, this code provides a simple implementation of a deep neural network using Keras for the Fashion MNIST dataset with an accuracy of over 88%.

# Word Recognizer

The perceptron is a simple neural network capable of classifying input data based on linear transformations. In this project, we use a perceptron to solve the task of handwritten word recognition.

## Architecture
The perceptron consists of the following main components:

#### 1. Input Layer
Represents the vectorized image of a handwritten word. Each pixel of the image corresponds to one input neuron.
#### 2. Hidden Layer
Contains neurons that perform linear transformations on the input data. The weights of these transformations are learned during the training process.
#### 3. Output Layer
Determines the probabilities of the input image belonging to different classes (individual words). The number of neurons in the output layer is equal to the number of classes (words) in the training set.

## Training
The training of the perceptron proceeds as follows:
#### 1. Data Preparation
Handwritten word images are converted to vectors and split into training and test sets.
#### 2. Weight Initialization
The weights of the connections between the perceptron layers are initialized with random values.
#### 3. Iterative Training
For each image in the training set:
* The image is fed into the perceptron.
* The output signal of the perceptron is computed.
* The output signal is compared with the desired response (the true class label).
* The Perceptron Learning Rule is applied to update the connection weights.
#### 4. Performance Evaluation
The trained perceptron is tested on the test set, and the recognition accuracy is computed.

## Application
I have developed a Qt Creator application that allows users to interact with the handwritten word recognition model. The key features of the application are:

### File Upload and Recognition
Users can upload an image file containing handwritten words. The application will then use the trained perceptron model to recognize the words in the image and display the results.

### Model Training
Users can also choose to train the perceptron model themselves. The application allows them to specify the training and test data paths, as well as the number of training iterations and other hyperparameters.

## Prerequisites
* GCC
* QtCreator

## Author
This application was developed by Alexander Mynzul.

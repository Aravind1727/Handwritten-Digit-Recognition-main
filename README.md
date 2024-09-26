# Handwritten Digit Recognition using Convolutional Neural Networks (CNN)
This project demonstrates Handwritten-Digit(0-9)-Recognition using (CNN) Convolutional Neural Networks.
## Dataset
The project uses the famous MNIST dataset, which consists of 60,000 labeled images of handwritten digits for training and 10,000 labeled images for testing. Each image is 28x28 pixels in size and grayscale, with pixel values ranging from 0 to 255. The dataset is preprocessed to normalize pixel values.
## Model Architecture
* The first layer is a convolutional layer (Conv2D) with 32 filters, a kernel size of (3, 3), and a ReLU activation function. It takes an input image of shape (28, 28, 1) where 1 represents grayscale channel.
* The output from the convolutional layer is then passed through a max pooling layer (MaxPooling2D) with a pool size of (2, 2), which helps reduce spatial dimensions while preserving important features.
* Another convolutional layer with 64 filters, a kernel size of (3, 3), and a ReLU activation function is added, followed by another max pooling layer with a pool size of (2, 2).
* The output from the last max pooling layer is then flattened into a 1D array using a Flatten layer, which prepares the data for the fully connected layers.
* Two fully connected layers (Dense) are added on top of the flattened output. The first dense layer has 128 units with a ReLU activation function, while the second dense layer has 10 units with a softmax activation function, which gives the probability of each class (0 to 9) being the correct digit.

## Model Evaluation
![1](https://github.com/Aravind1727/Handwritten-Digit-Recognition-main/tree/9529886aad2baa98d4a60f2e8188977e677c76f0/prediction)

## Model Deployment
### Streamlit Front-end
The Streamlit front-end provides a simple and interactive web-based user interface for users to draw digit and get predictions from the trained CNN model.

1. Draw a digit on a canvas: Users can use the mouse or touchpad to draw a digit on a canvas provided by the Streamlit app. The drawn image is then passed to the trained CNN model for prediction.
2. Display prediction results: The Streamlit app displays the predicted digit.

## Sample Output
u can check here in the githb repository....

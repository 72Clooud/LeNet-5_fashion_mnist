# LeNet-5_fashion_mnist
This repository contains a LeNet-5 inspired convolutional neural network for classifying Fashion MNIST images using TensorFlow and Keras.
# Dataset
The Fashion MNIST dataset consists of 60,000 training images and 10,000 test images of clothing items, each in one of 10 categories. Images are preprocessed by normalizing pixel values to [0, 1] and reshaping them to (28, 28, 1).
# Model Architecture
The model architecture includes:

1. Conv2D: 32 filters, 5x5 kernel, ReLU activation
2. MaxPooling2D: 2x2 pool size
3. Conv2D: 64 filters, 5x5 kernel, ReLU activation
4. MaxPooling2D: 2x2 pool size
5. Flatten
6. Dense: 120 units, ReLU activation
7. Dense: 84 units, ReLU activation
8. Dense: 10 units, softmax activation

# Data Augmentation
Data augmentation is applied using ImageDataGenerator with:
* Rotation: 30 degrees
* Width/height shift: 20%
* Zoom: 20%
* Horizontal flip
* Nearest fill mode
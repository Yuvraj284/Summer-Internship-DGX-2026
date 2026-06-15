# Day 05 – Convolutional Neural Networks (CNN)

## Introduction

Convolutional Neural Networks (CNNs) are a specialized type of Artificial Neural Network designed primarily for image processing and computer vision tasks.

Traditional neural networks work well for structured data but become inefficient when handling images because images contain a large number of pixels and spatial relationships.

CNNs solve this problem by automatically learning important visual features such as edges, shapes, textures, and patterns directly from images.

CNNs are widely used in:

* Image Classification
* Object Detection
* Facial Recognition
* Medical Image Analysis
* Self-Driving Cars
* Handwritten Digit Recognition

---

## Why CNN Instead of Traditional Neural Networks?

Consider a grayscale image of size:

28 × 28

Total pixels:

28 × 28 = 784

A traditional neural network treats all pixels independently and ignores spatial relationships between neighboring pixels.

CNNs preserve spatial information and learn local patterns efficiently using convolution operations.

This makes CNNs faster, more accurate, and more suitable for image-related tasks.

---

## Architecture of a CNN

A Convolutional Neural Network generally consists of the following layers:

Input Layer

↓

Convolution Layer

↓

Activation Function

↓

Pooling Layer

↓

Flatten Layer

↓

Fully Connected Layer

↓

Output Layer

Each layer performs a specific operation to gradually extract meaningful information from the image.

---

# Input Layer

The Input Layer receives image data.

For the MNIST dataset:

* Image Size = 28 × 28
* Grayscale Image
* Channel = 1

Input Shape:

(28, 28, 1)

The pixel values are usually normalized between 0 and 1 before training.

---

# Convolution Layer

The Convolution Layer is the most important component of a CNN.

It uses small filters (kernels) that slide across the image and extract important features.

Examples of features detected:

* Edges
* Corners
* Curves
* Shapes
* Textures

Instead of learning from individual pixels, CNNs learn meaningful visual patterns.

Common filter sizes:

* 3 × 3
* 5 × 5

Example:

Conv2D(32, (3,3))

This means:

* 32 filters
* Each filter size = 3 × 3

---

# Activation Function

After convolution, an activation function is applied.

The most commonly used activation function is ReLU.

ReLU (Rectified Linear Unit):

Output = 0 for negative values

Output = x for positive values

Advantages:

* Fast computation
* Reduces training time
* Helps neural networks learn complex patterns

---

# Pooling Layer

Pooling reduces the size of feature maps.

The most common pooling technique is Max Pooling.

Example:

2 × 2 Max Pooling

The maximum value from each 2 × 2 region is selected.

Benefits:

* Reduces computational cost
* Reduces overfitting
* Retains important features

Example:

MaxPooling2D((2,2))

---

# Flatten Layer

After several convolution and pooling operations, the feature maps are converted into a one-dimensional vector.

This process is called Flattening.

Example:

Feature Map

↓

Flatten

↓

Vector

This vector is then passed to fully connected layers.

---

# Fully Connected Layer

The Fully Connected Layer works similarly to a traditional neural network.

Its purpose is:

* Learn high-level patterns
* Perform classification

Example:

Dense(128, activation='relu')

This layer contains 128 neurons.

---

# Output Layer

The Output Layer generates the final prediction.

For MNIST:

Digits = 0 to 9

Total Classes = 10

Therefore:

Dense(10, activation='softmax')

Softmax converts outputs into probabilities.

Example:

Digit 0 → 1%

Digit 1 → 2%

Digit 5 → 92%

Digit 8 → 3%

The class with the highest probability becomes the prediction.

---

# Dropout Layer

Dropout is a regularization technique used to reduce overfitting.

During training, some neurons are randomly ignored.

Example:

Dropout(0.5)

This means approximately 50% of neurons are temporarily deactivated during training.

Benefits:

* Better generalization
* Reduced overfitting
* Improved model robustness

---

# MNIST Dataset

MNIST stands for Modified National Institute of Standards and Technology Dataset.

Dataset Details:

* Total Images = 70,000
* Training Images = 60,000
* Testing Images = 10,000
* Classes = 10
* Digits = 0–9
* Image Size = 28 × 28

MNIST is considered the "Hello World" dataset of Deep Learning.

---

# Training a CNN

The training process involves:

1. Forward Propagation
2. Loss Calculation
3. Backpropagation
4. Weight Update
5. Repeat for Multiple Epochs

The objective is to minimize prediction error and maximize classification accuracy.

---

# Loss Function

For multi-class classification problems such as MNIST:

Sparse Categorical Crossentropy

is commonly used.

The loss function measures how far the predictions are from the actual labels.

Lower loss indicates better performance.

---

# Optimizer

The optimizer updates network weights during training.

One of the most widely used optimizers is:

Adam Optimizer

Advantages:

* Fast convergence
* Adaptive learning rate
* Excellent performance in Deep Learning applications

---

# Handwritten Digit Recognition

In this experiment, a CNN was trained using the MNIST dataset to recognize handwritten digits.

The trained model was further extended to classify custom digit images uploaded by the user.

This demonstrates a real-world application of Deep Learning and Computer Vision.

---

# Advantages of CNN

* Automatic feature extraction
* High image classification accuracy
* Efficient parameter sharing
* Reduced manual preprocessing
* Excellent performance on visual data

---

# Limitations of CNN

* Requires large datasets
* Computationally expensive
* Training can take significant time
* Sensitive to image quality and preprocessing

---

# Conclusion

Convolutional Neural Networks are one of the most important architectures in Deep Learning and Computer Vision. They automatically learn visual features from images and achieve high accuracy in classification tasks. In this activity, a CNN was successfully trained on the MNIST dataset and used for handwritten digit recognition, including prediction of user-uploaded digit images.
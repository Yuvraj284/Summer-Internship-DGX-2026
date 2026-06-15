# Day 05 - Convolutional Neural Network (CNN) on MNIST Dataset

## Objective

The objective of this activity was to understand the working of Convolutional Neural Networks (CNNs) and apply them to the problem of digit recognition using the MNIST dataset.

In addition to training and evaluating the CNN model, a custom digit prediction feature was implemented to classify user-uploaded digit images.

---

## Topics Covered

* Introduction to Convolutional Neural Networks (CNN)
* Convolution Layer
* Activation Functions (ReLU)
* Pooling Layer
* Flatten Layer
* Fully Connected Layer
* Softmax Classification
* Model Training and Evaluation
* Image Classification
* Digit Recognition using CNN

---

## Dataset Used

### MNIST Dataset

The MNIST dataset is one of the most widely used benchmark datasets in Deep Learning and Computer Vision.

Dataset Details:

* Total Images: 70,000
* Training Images: 60,000
* Testing Images: 10,000
* Image Size: 28 × 28 Pixels
* Grayscale Images
* Classes: 10 (Digits 0–9)

---

## Why MNIST?

MNIST is considered the "Hello World" dataset of Deep Learning because it provides a simple and effective introduction to image classification.

The dataset helps in understanding:

* Neural Networks
* Convolutional Neural Networks
* Feature Extraction
* Computer Vision
* Classification Tasks

---

# CNN Architecture

The following CNN architecture was implemented:

Input Layer

↓

Conv2D (32 Filters, 3×3)

↓

MaxPooling2D

↓

Conv2D (64 Filters, 3×3)

↓

MaxPooling2D

↓

Flatten Layer

↓

Dense Layer (128 Neurons)

↓

Dropout Layer (0.5)

↓

Output Layer (10 Classes)

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Loading the MNIST dataset
2. Normalizing pixel values from 0–255 to 0–1
3. Reshaping images to (28, 28, 1)
4. Preparing the data for CNN training

---

## Model Compilation

Optimizer:

* Adam Optimizer

Loss Function:

* Sparse Categorical Crossentropy

Evaluation Metric:

* Accuracy

---

## Model Training

The CNN model was trained for 10 epochs using the MNIST training dataset.

Training included:

* Forward Propagation
* Loss Calculation
* Backpropagation
* Weight Updates using Adam Optimizer

---

## Results

### Training Accuracy

Approximately:

99.27%

### Validation Accuracy

Approximately:

99.16%

The model achieved excellent performance on the MNIST dataset and demonstrated strong generalization capability.

---

## Confusion Matrix

A confusion matrix was generated to evaluate model predictions across all digit classes.

The results indicated that most digits were classified correctly, with only a small number of misclassifications.

---

## Custom Digit Prediction

A custom prediction feature was implemented that allows users to upload their own digit images.

Workflow:

1. Upload Image
2. Convert to Grayscale
3. Resize to 28 × 28
4. Normalize Pixel Values
5. Reshape for CNN Input
6. Predict Digit using the Trained Model

---

## Test Image

A sample custom image was tested:

* `test_photo5.jpeg`

The image was preprocessed and passed through the trained CNN model for digit prediction.

The experiment demonstrated that the model can classify user-uploaded digit images after appropriate preprocessing and resizing.

---

## Libraries Used

* NumPy
* Matplotlib
* TensorFlow
* Keras
* Scikit-Learn
* Seaborn
* Pillow (PIL)

---

## Files Included

* CNN_MNIST_Digit_Recognition.ipynb
* Notes.md
* README.md
* test_photo5.jpeg

---

## Learning Outcomes

After completing this activity, I learned:

* The architecture and working of CNNs.
* The role of convolution and pooling layers.
* How feature extraction is performed automatically.
* The importance of activation functions such as ReLU.
* How CNNs are trained using backpropagation.
* How image classification models are evaluated.
* How to preprocess images for prediction.
* How to build a practical digit recognition system using Deep Learning.

---

## Conclusion

This activity provided practical experience with Convolutional Neural Networks and image classification. A CNN model was successfully trained on the MNIST dataset and achieved high classification accuracy. The project was further extended with a custom digit prediction feature, demonstrating how Deep Learning models can be applied to real-world image recognition tasks.
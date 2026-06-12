# Day 02 - Machine Learning Algorithms

## Objective

The objective of this activity was to gain practical experience with supervised machine learning algorithms and understand the difference between regression and classification problems.

Three machine learning algorithms were implemented and evaluated using real-world datasets.

---

## Algorithms Implemented

### 1. Linear Regression

Linear Regression was implemented on the Energy Consumption Dataset to predict continuous numerical values.

#### Dataset Features

* Building Type
* Square Footage
* Number of Occupants
* Appliances Used
* Average Temperature
* Day of Week

#### Target Variable

* Energy Consumption

#### Concepts Learned

* Data Preprocessing
* Feature Selection
* Train-Test Split
* Model Training
* Prediction
* R² Score Evaluation

---

### 2. Support Vector Machine (SVM)

Support Vector Machine was implemented on the Iris Dataset for multiclass classification.

#### Dataset Features

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

#### Target Classes

* Iris-setosa
* Iris-versicolor
* Iris-virginica

#### Concepts Learned

* Classification
* Hyperplane
* Maximum Margin Separation
* Accuracy Evaluation
* Confusion Matrix
* Classification Report

#### Results

The SVM classifier achieved excellent performance on the Iris dataset and successfully classified all test samples.

Performance Metrics:

* Accuracy: 100%
* Precision: 100%
* Recall: 100%
* F1-Score: 100%

---

### 3. Random Forest Classifier

Random Forest was implemented on the Iris Dataset to classify flower species using an ensemble of Decision Trees.

#### Concepts Learned

* Decision Trees
* Ensemble Learning
* Majority Voting
* Feature-Based Classification
* Model Evaluation

---

## Datasets Used

### Energy Consumption Dataset

Used for the regression task.

Objective:
Predict energy consumption based on building characteristics and environmental factors.

### Iris Dataset

Used for classification tasks.

Objective:
Predict the species of a flower based on sepal and petal measurements.

---

## Libraries Used

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

## Workflow Followed

1. Load and inspect the dataset.
2. Perform basic preprocessing.
3. Select input features and target variable.
4. Split the dataset into training and testing sets.
5. Train the machine learning model.
6. Generate predictions.
7. Evaluate model performance using appropriate metrics.
8. Analyze the results.

---

## Learning Outcomes

After completing this activity, I learned:

* The difference between regression and classification problems.
* How Linear Regression predicts continuous numerical values.
* How Support Vector Machines classify data using optimal decision boundaries.
* How Random Forest combines multiple Decision Trees to improve prediction accuracy.
* How to evaluate machine learning models using accuracy, precision, recall, F1-score, and R² score.
* The importance of train-test splitting for model validation.

---

## Files Included

* Linear_Regression_Energy.ipynb
* SVM_Iris.ipynb
* Random_Forest_Iris.ipynb
* Energy Consumption Dataset
* Iris Dataset

---

## Conclusion

This activity provided practical exposure to supervised machine learning algorithms used for both regression and classification tasks. Through the implementation of Linear Regression, Support Vector Machine, and Random Forest, a strong foundation was developed in model training, prediction, and performance evaluation.
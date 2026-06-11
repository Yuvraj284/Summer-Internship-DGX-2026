# Day 02 - Linear Regression on Energy Consumption Dataset

## Objective

The objective of this activity was to implement Linear Regression and understand how machine learning models can be used to predict continuous numerical values.

## Dataset

Dataset Used: Energy Consumption Dataset

The dataset contains information about buildings and their energy usage, including:

* Building Type
* Square Footage
* Number of Occupants
* Appliances Used
* Average Temperature
* Day of Week
* Energy Consumption (Target Variable)

## Concepts Covered

### Data Preprocessing

* Loading CSV files using Pandas
* Understanding dataset structure
* Handling categorical features using encoding

### Feature Selection

Input Features:

* Building Type
* Square Footage
* Number of Occupants
* Appliances Used
* Average Temperature
* Day of Week

Target Variable:

* Energy Consumption

### Train-Test Split

The dataset was divided into:

* 80% Training Data
* 20% Testing Data

### Linear Regression

A Linear Regression model was trained to learn the relationship between building characteristics and energy consumption.

### Model Evaluation

The model was evaluated using:

* R² Score
* Actual vs Predicted Comparison

## Libraries Used

* Pandas
* NumPy
* Matplotlib
* Scikit-Learn

## Workflow

1. Load the dataset.
2. Perform basic preprocessing.
3. Encode categorical variables.
4. Split the dataset into training and testing sets.
5. Train a Linear Regression model.
6. Generate predictions.
7. Evaluate model performance.
8. Visualize results.

## Learning Outcomes

After completing this activity, I learned:

* The difference between supervised and unsupervised learning.
* The concept of regression problems.
* How Linear Regression works.
* How to train a machine learning model.
* How to generate predictions using unseen data.
* How to evaluate model performance using R² Score.

## Files Included

* LinearRegression_Day02_11_06_2026.ipynb
* train_energy_data.csv
* test_energy_data.csv
* README.md

## Conclusion

Linear Regression was successfully implemented on the Energy Consumption dataset. The model was trained using historical data and used to predict energy consumption values. This activity provided practical exposure to supervised machine learning and regression analysis.

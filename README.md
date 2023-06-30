# Power Monitoring System

## Introduction

The Power Monitoring System is a project aimed at monitoring and analyzing the electrical power consumption of a building, facility, or specific equipment. The system provides valuable insights into energy usage patterns, identifies areas of inefficiency, and enables better energy management and cost savings. This documentation serves as a comprehensive guide to understand and utilize the Power Monitoring System implemented using Python.

![image](https://github.com/VD0023/PowerMonitoringSystem/assets/99820386/1ac1417e-dc73-43e3-b1e3-c293e582384e)


## Table of Contents

1. Installation
2. Dataset Overview
3. Data Preprocessing
4. Exploratory Data Analysis
5. Machine Learning Algorithm Evaluation
6. Training and Testing the ML Algorithm
7. Usage and Predictions

## 1. Installation

To use the Power Monitoring System, follow these installation steps:

1. Install Python: Download and install Python from the official Python website (https://www.python.org) based on your operating system.
2. Install Required Libraries: Open a command prompt or terminal and run the following command to install the necessary libraries:
   ```
   pip install pandas matplotlib scikit-learn
   ```

## 2. Dataset Overview

The Power Monitoring System utilizes a dataset that contains information about voltage, current, power, and corresponding classes. The dataset is provided in a CSV file format named "Energy Meter.csv" and includes the following columns:

- Voltage: The voltage measurement in the electrical system.
- Current: The current measurement in the electrical system.
- Power: The power consumption in the electrical system.
- Class: The class label corresponding to the power measurement.

## 3. Data Preprocessing

The project begins with data preprocessing to prepare the dataset for analysis. The following steps are performed:

- Loading the Dataset: The CSV file is read using the pandas library's `read_csv` function, and column names are assigned accordingly.
- Splitting Data: The dataset is split into input features (voltage, current, and power) denoted by 'X' and the target variable (class) denoted by 'y'.

## 4. Exploratory Data Analysis

Exploratory Data Analysis (EDA) is conducted to gain insights into the dataset. The following visualizations are generated:

- Bar Plot: Visualizes the dataset using bar plots, providing a graphical representation of the data distribution.
- Histogram Plot: Displays the distribution of individual variables using histograms.
- Scatter Plot Matrix: Shows the relationship between variables using scatter plots.

![image](https://github.com/VD0023/PowerMonitoringSystem/assets/99820386/f60ad577-a73a-4bc1-a7ba-fea52d7e76d0)


## 5. Machine Learning Algorithm Evaluation

To determine the most suitable machine learning algorithm for the Power Monitoring System, the dataset is evaluated using various algorithms. The following algorithms are implemented:

- Logistic Regression
- Linear Discriminant Analysis
- K-Nearest Neighbors
- Decision Tree Classifier
- Gaussian Naive Bayes
- Support Vector Machines (SVM)

The algorithms are evaluated using cross-validation and accuracy scores to compare their performance.

## 6. Training and Testing the ML Algorithm

The chosen machine learning algorithm is trained and tested using the following steps:

- Splitting Data: The dataset is split into training and validation sets using the `train_test_split` function from scikit-learn.
- Model Training: The selected algorithm (SVM in this case) is trained on the training data using the `fit` method.
- Model Persistence: The trained model is saved in a file named "finalized_model.pkl" using the pickle library.
- Model Evaluation: The model's accuracy is evaluated using the validation dataset to assess its performance.

## 7. Usage and Predictions

Once the model is trained and saved, it can be used for making predictions on new data. The following steps outline the process:

- Loading the Model: The saved model is loaded from the "finalized_model.pkl" file using the pickle library.
- Predicting Values: New input data (voltage

, current, and power) can be provided as a list to obtain predictions from the loaded model.
- Obtaining Results: The predicted class labels are obtained as output, which can be used for further analysis or decision-making.

---

With this comprehensive documentation, you should now have a solid understanding of the Power Monitoring System and its implementation using Python. You can utilize this system to monitor and analyze power consumption patterns, identify areas of inefficiency, and optimize energy management for cost savings.

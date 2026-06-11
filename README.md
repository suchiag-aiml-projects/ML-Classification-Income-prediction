# ML-Classification-Income-prediction

Using various classification models to predict which model gives more accuracy in predicting the income of an adult.

## Project Overview
In this repository, you will find the classification models are used to predict if the Income of an adult is >50k or <50k.
This project uses various classification models to find which model works best to find the income of a person based on various factor like 
age,workclass,education,marital-status,occupation, relationship, race, sex, capital-gain,capital-loss,hours-per-week and native-country.
- The models used in this prediction are:
- Logistic Regression
- K-Nearest Neighbors
- Support Vector Machine SVM Model
- Kernel SVM
- Naive Bayes 
- Decision Tree Classification
- Random Forest Classification
- XGBoost

## Project Objectives

Predict whether annual income of an individual exceeds $50K/yr based on census data. Also known as "Census Income" dataset.
This prediction helps to study and determine income inequality based on various factors like Gender,Race,Education, Age etc.

Link to the dataset: https://archive.ics.uci.edu/dataset/2/adult

## Project Phases

### Data Cleaning & Analysis
- There are no null values in the dataset.
- Column names were added from a seperate file adult.names.

### Data Preprocessing & Feature Engineering
- After splitting the data into train and test set, there 8 columns with categorical values. And most of the columns have multiple distinct values.
- Since after applying OneHotEncoding each column produce multiple column, param value drop = 'first' was applied to avoid ### dummy variable trap ### and also
  it reduces few number of columns.
- Standard Scalar was applied to the remaining numerical value data.
- Dependent variable with value of income >50k or <50k, here labelEncoding was applied with value of '>50k' as 1, and '<50k' as 0.

### Model Selection & Fine Tuning
- Training multiple models like Linear Regression, Naive-Bayes, Kernel-SVM, Decision Tree, Random Forest, and XGBoost.
- There was performance improvement in XGBoost after tuning Hyperparameter from 86.7 to 87%.

### Observation and Conclusion
- It has 32,561 instances and 14 features — not too small, not too large — making it ideal for showcasing ML skills. The feature types include both categorical      and integer columns, and it contains missing values.

adult-income-classification/
│
├── data/
│   └── adult.csv
│   └── adult.names    
│
├── notebooks/
│   └── Adult_Income_Classification.jpynb
│
└── README.md

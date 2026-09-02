# Breast Cancer Classification with SGDClassifier

## Overview

This project focuses on breast cancer classification using the Breast Cancer dataset from Scikit-learn.

The main goal of this project is to investigate the impact of feature standardization on the performance of an SGDClassifier. The model is trained and evaluated using both the original data and standardized data, allowing for a comparison of their scores and overall performance.

## Dataset

The dataset is loaded using Scikit-learn's built-in `load_breast_cancer` function.

* Number of samples: 569
* Number of features: 30
* Task: Binary classification

## Project Steps

1. Load the Breast Cancer dataset.
2. Split the dataset into training and testing sets.
3. Train the model using the original data.
4. Standardize the features using `StandardScaler`.
5. Train the model again using the standardized data.
6. Evaluate and compare the model scores.
7. Analyze the impact of feature scaling on model performance.

## Feature Standardization

The project uses `StandardScaler` to standardize the input features.

Standardization helps transform features to a similar scale, which can be particularly important for algorithms such as `SGDClassifier` that use gradient-based optimization.

The main comparison in this project is:

* Model performance without feature standardization.
* Model performance after feature standardization.

This comparison demonstrates how data scaling can affect the model's score and classification performance.

## Technologies Used

* Python
* Scikit-learn
* Jupyter Notebook

## Libraries Used

```python
from sklearn.datasets import load_breast_cancer
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import SGDClassifier
```

## Model

The classification model used in this project is:

* `SGDClassifier`

The model is trained using logistic regression loss for binary classification.

## Results

The results allow us to compare the performance of the model before and after feature standardization.

The main purpose is to observe whether standardizing the features improves the model's score and to understand the importance of feature scaling when using gradient-based machine learning algorithms.

## Conclusion

This project demonstrates that data preprocessing can have a significant impact on machine learning model performance. By comparing standardized and non-standardized data, we can better understand how feature scaling affects the learning process and the final model score.


# Breast Cancer Prediction

A machine learning project that compares Logistic Regression and Random Forest classifiers for breast cancer diagnosis prediction.

## Project Overview

The goal of this project is to build and evaluate machine learning classification models to distinguish between benign and malignant breast cancer cases based on numerical tumor features.

## Models

Two classification algorithms were implemented:

- Logistic Regression
- Random Forest Classifier

MinMaxScaler was integrated into a Scikit-learn Pipeline for Logistic Regression. Random Forest was trained without feature scaling.

## Data Preprocessing

The preprocessing steps included:

- Converting diagnosis labels into numerical values:
  - Benign = 0
  - Malignant = 1
- Separating features and target labels
- Splitting the dataset into training and testing sets
- Using stratified sampling to preserve class proportions

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Results

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 97.37% | 96.49% |
| Precision | 1.0000 | 1.0000 |
| Recall | 0.9286 | 0.9048 |
| F1-score | 0.9630 | 0.9500 |

Logistic Regression achieved slightly better results on the selected test set.

Both models achieved a precision score of 1.00. However, Logistic Regression identified 39 out of 42 malignant cases, while Random Forest identified 38 out of 42.

Further evaluation using cross-validation would be useful to assess model stability.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
Breast-Cancer-Prediction/
│
├── breast_cancer_prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Dataset

The dataset file is not included in this repository.

Please refer to the original dataset source and its licensing terms before downloading or using it.

## Disclaimer

This project is for educational purposes only and is not intended for medical diagnosis or clinical decision-making.
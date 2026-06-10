# Heart Disease Prediction Model

## Overview

This project builds a machine learning model to predict the severity level of heart disease using patient medical attributes such as age, cholesterol, resting blood pressure, maximum heart rate, and other clinical features.

The project compares multiple classification models and selects the best model based on validation performance.

## Dataset

The dataset is taken from the **UCI Machine Learning Repository**.

- Dataset: Heart Disease Dataset
- Source: UCI Machine Learning Repository
- Task: Multiclass classification
- Target: Heart disease severity level
- Features: Medical and clinical attributes of patients

Dataset URL: https://archive.ics.uci.edu/dataset/45/heart+disease

## Models Used

The following models are trained and compared:

- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)

Hyperparameter tuning is performed using **GridSearchCV** with stratified 5-fold cross-validation.

## Methodology

The project follows these steps:

1. Load the UCI Heart Disease dataset
2. Explore dataset structure, missing values, and target distribution
3. Perform exploratory data analysis using visualizations
4. Split the data into training, validation, and test sets
5. Preprocess numerical and categorical features
6. Train and tune classification models
7. Compare models using validation performance
8. Evaluate the final model on the test set
9. Display confusion matrix and ROC curves

## Data Split

The dataset is divided into:

- Training set: 70%
- Validation set: 10%
- Test set: 20%

## Preprocessing

The preprocessing pipeline includes:

- Median imputation for numerical features
- Standard scaling for numerical features
- Most frequent imputation for categorical features
- One-hot encoding for categorical features

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- F1 Macro Score
- ROC-AUC Score
- Classification Report
- Confusion Matrix
- One-vs-Rest ROC Curves

## Best Model

Based on validation and test performance, **Logistic Regression** was selected as the best model.

### Final Test Results

- Accuracy: `0.639344`
- F1 Macro: `0.353641`
- AUC: `0.857866`

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- ucimlrepo

## How to Run

Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo
```

Run the Jupyter Notebook:

```bash
jupyter notebook Heart_Disease_Prediction_Model.ipynb
```

## Project Structure

```bash
.
├── Heart_Disease_Prediction_Model.ipynb
├── README.md
└── requirements.txt
```

## Conclusion

The project shows how machine learning can be used to classify heart disease severity levels using clinical data. Among the tested models, Logistic Regression performed best and achieved a strong AUC score, although the macro F1 score suggests that some classes are harder to predict than others.

## Author

Awais Ahmed Channa

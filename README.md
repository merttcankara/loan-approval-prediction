# Loan Approval Prediction

## Project Overview

This project focuses on building a machine learning classification model to predict whether a loan application will be approved or rejected. The goal is to support faster, more consistent, and data-driven loan evaluation decisions.

## Business Problem

Loan approval decisions are important for financial institutions because they require accurate and consistent evaluation of applicants. In this project, applicant information such as income, loan amount, credit history, education, employment status, and property area was used to predict loan approval status.

## Dataset

The dataset contains 614 observations and 13 variables. The target variable is `Loan_Status`, which shows whether a loan application was approved or not.

Main features include:

- Gender
- Married
- Dependents
- Education
- Self_Employed
- ApplicantIncome
- CoapplicantIncome
- LoanAmount
- Loan_Amount_Term
- Credit_History
- Property_Area

## Project Workflow

The project follows a complete machine learning workflow:

1. Data overview and initial inspection
2. Exploratory data analysis
3. Missing value analysis and imputation
4. Feature engineering
5. Categorical encoding
6. Train-test split
7. Feature scaling for Logistic Regression
8. Model training and comparison
9. Hyperparameter tuning with GridSearchCV
10. Final model selection

## Models Used

The following classification models were compared:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

## Model Evaluation

The models were evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Cross-validation accuracy

## Results

Logistic Regression achieved the best overall performance among the baseline models.

After hyperparameter tuning, Logistic Regression and Random Forest achieved similar test results. Logistic Regression was selected as the final model because it is simple, interpretable, and computationally efficient.

## Final Model

The final selected model is Logistic Regression.

Final model performance:

- Accuracy: 85.4%
- Precision: 83.2%
- Recall: 98.8%
- F1 Score: 90.3%

## Key Insights

- Credit history appeared to be one of the strongest predictors of loan approval.
- Logistic Regression performed strongly despite its simplicity.
- Hyperparameter tuning improved cross-validated F1 score but did not improve the final test metrics.
- A simple and interpretable model was more suitable for this dataset than more complex tree-based models.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Files

- `loan_prediction_Mertcan_Kara.ipynb`: Main notebook containing the full analysis and modeling process.
- `Mertcan_Kara_Loan_Predict.pdf`: Project report.

## Conclusion

This project demonstrates a complete machine learning workflow for a binary classification problem. The final Logistic Regression model provides a strong balance between performance, interpretability, and efficiency.

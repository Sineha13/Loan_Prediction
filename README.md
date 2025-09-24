# Loan Prediction ML Project
This project predicts whether a loan application will be approved or not using machine learning. The model is trained on a dataset of applicants’ personal and financial information and provides predictions based on input features.

## Dataset
- Rows: 614
- Columns: 13
- Key Features: Gender, Married, Dependents, Education, Self_Employed, ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Property_Area
- Target: Loan_Status (Y/N)

## Data Preprocessing
-Dropped missing values.
-Converted categorical variables into numerical values (e.g., Gender: Male=1, Female=0).
-Replaced 3+ in Dependents with 4.
-Label encoded the target variable (Y → 1, N → 0).

## Exploratory Data Analysis (EDA)
-Visualized distributions of key features.
-Checked correlations between features and loan approval status.

## Machine Learning Models
-Logistic Regression
-Support Vector Machine (SVM)
-Decision Tree Classifier
-Random Forest Classifier (best performing)

## Model Training & Evaluation
-Used train-test split (80-20) and K-Fold Cross Validation.
-Random Forest achieved highest accuracy (~81%).
-Hyperparameter tuning applied to Random Forest using RandomizedSearchCV.

## Results
Random Forest Classifier provided the best prediction performance with cross-validation score ~80.6%.

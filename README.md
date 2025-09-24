# employee_attrition-model
predicting employee attrition

Employee Attrition Prediction

This project contains a machine learning workflow to predict employee attrition. It demonstrates how to preprocess employee data, train a Random Forest model, and evaluate its performance.

Dataset

employee_attrition.csv

Features include: Education, City, PaymentTier, Age, Gender, EverBenched, ExperienceInCurrentDomain, and target LeaveOrNot.

Steps Performed

Data Exploration – checked info, descriptive statistics, and null values.

Data Preprocessing – encoded categorical variables (City, Gender, EverBenched) and scaled numeric features.

Train-Test Split – split data into training and test sets.

Model Training – trained a Random Forest Classifier.

Evaluation – calculated accuracy, precision, recall, and F1-score.

Optional – handled class imbalance using SMOTE.

Results
Random Forest (Before Balancing)

Accuracy: ~0.76

Class 0 (Stayed): Precision = 0.77 | Recall = 0.91 | F1 = 0.84

Class 1 (Left): Precision = 0.75 | Recall = 0.48 | F1 = 0.58

Random Forest (After Balancing / SMOTE)

Accuracy: ~0.74

Class 0 (Stayed): Precision = 0.71 | Recall = 0.82 | F1 = 0.76

Class 1 (Left): Precision = 0.78 | Recall = 0.66 | F1 = 0.72

Balancing significantly improved recall for employees likely to leave, which is critical for HR decision-making.

How to Run

Open employee_attrition.ipynb in Jupyter Notebook or Google Colab.

Install required libraries: pandas, scikit-learn, joblib.

Run cells sequentially to train the model and evaluate performance.

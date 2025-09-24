# Employee Attrition Prediction

This project contains a **machine learning workflow to predict employee attrition**. It demonstrates data preprocessing, model training using Random Forest, and evaluation of model performance.

---

## Dataset
- File: `Employee`
- Features include: `Education`,'JoiningYear', `City`, `PaymentTier`, `Age`, `Gender`, `EverBenched`, `ExperienceInCurrentDomain`
- Target: `LeaveOrNot`

---

## Steps Performed
1. **Data Exploration** – checked info, descriptive statistics, and null values.  
2. **Data Preprocessing** – encoded categorical variables (`City`, `Gender`, `EverBenched`) and scaled numeric features.  
3. **Train-Test Split** – split data into training and test sets.  
4. **Model Training** – trained a **Random Forest Classifier**.  
5. **Evaluation** – calculated accuracy, precision, recall, and F1-score.  
6. **Optional** – handled class imbalance using SMOTE.

---

## Results

### Random Forest (Before Balancing)
- Accuracy: ~0.76  
- **Class 0 (Stayed)**: Precision = 0.77 | Recall = 0.91 | F1 = 0.84  
- **Class 1 (Left)**: Precision = 0.75 | Recall = 0.48 | F1 = 0.58  

### Random Forest (After Balancing / SMOTE)
- Accuracy: ~0.74  
- **Class 0 (Stayed)**: Precision = 0.71 | Recall = 0.82 | F1 = 0.76  
- **Class 1 (Left)**: Precision = 0.78 | Recall = 0.66 | F1 = 0.72  

> Balancing improved recall for employees likely to leave, making the model more useful for HR decisions.

---

## How to Run
1. Open `employee_attrition.ipynb` in Jupyter Notebook or Google Colab.  
2. Install required libraries: `pandas`, `scikit-learn`, `joblib`.  
3. Run cells sequentially to train the model and evaluate performance.

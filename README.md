# Credit Card Approval Prediction

This project predicts whether a credit card application will be **approved or rejected** based on applicant details.  
It uses the **UCI Credit Approval dataset** and applies **Logistic Regression** for classification.  

---

## Dataset
- Source: [UCI Machine Learning Repository - Credit Approval Dataset](https://archive.ics.uci.edu/ml/datasets/credit+approval)
- Contains categorical and numerical features about credit card applicants.
- Missing values are represented as `?` and are handled using imputation.

---

## Project Workflow
1. **Load dataset** and replace missing values (`?`) with `NaN`.  
2. **Impute missing values**:
   - Numerical features → filled with mean.  
   - Categorical features → filled with most frequent value.  
3. **Encode categorical features** using one-hot encoding (`pd.get_dummies`).  
4. **Split dataset** into training and test sets.  
5. **Feature scaling** using `StandardScaler`.  
6. **Train Logistic Regression model**.  
7. **Evaluate model**:
   - Confusion matrix  
   - Accuracy score  
   - GridSearchCV for hyperparameter tuning  

---

## Results
- The best logistic regression model achieved an accuracy of around **XX%** on the test set.  
- Evaluation metrics: confusion matrix, accuracy, precision, recall, F1-score.  

---

## Requirements
Install the required libraries with:

```bash
pip install -r requirements.txt

# customer-churn-prediction
Churn prediction project using Python, Logistic Regression &amp; Random Forest
# Customer Churn Prediction

## Project Overview
This project predicts customer churn for a telecom company using Python.  
It demonstrates **end-to-end data science workflow**: data cleaning, exploratory data analysis (EDA), feature encoding, scaling, model training, evaluation, and interpretation.

**Objective:** Identify customers likely to churn so the company can take preventive actions.

---

##  Dataset
- Source: Telecom customer data (fictional / Kaggle-style)
- Features include:
  - Demographics: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
  - Services: `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `StreamingTV`, etc.
  - Charges: `MonthlyCharges`, `TotalCharges`
  - Contract info: `Contract`, `PaperlessBilling`, `PaymentMethod`
- Target variable: `Churn` (1 = churned, 0 = stayed)

---

##  Tools & Libraries
- **Python**: main programming language
- **Pandas, NumPy**: data manipulation
- **Seaborn, Matplotlib**: visualization
- **Scikit-learn**: preprocessing, train-test split, modeling, evaluation
- **Models used**:
  - Logistic Regression
  - Random Forest Classifier

---

##  Methodology

1. **Exploratory Data Analysis (EDA)**
   - Visualized churn distribution
   - Compared numeric and categorical features with churn
   - Identified patterns and relationships

2. **Data Cleaning**
   - Converted `TotalCharges` to numeric
   - Filled missing values
   - Dropped irrelevant columns (`customerID`)

3. **Encoding Categorical Features**
   - Target mapped to 0/1
   - LabelEncoder for categorical features

4. **Feature Scaling**
   - StandardScaler applied to numeric features for model consistency

5. **Train-Test Split**
   - 80% training, 20% testing

6. **Model Training**
   - Logistic Regression
   - Random Forest (baseline)

7. **Evaluation**
   - Accuracy, precision, recall, F1-score
   - Confusion matrix
   - Feature importance interpretation

---

##  Key Results

**Logistic Regression**
- Accuracy: 81.5%
- Recall (churners): 58%
- F1-score (churners): 0.62
- Model coefficients indicate which features most influence churn

**Random Forest**
- Accuracy: 79.7%
- Recall (churners): 48%
- F1-score (churners): 0.55
- Feature importance shows which features drive churn predictions

> **Insight:** Logistic Regression performed better in identifying churners, making it more actionable for business decisions.

---

## Business Impact
- Predicting churn allows telecom companies to **proactively retain high-risk customers**
- Feature analysis guides **strategic actions** (e.g., offering discounts to high-risk customers)
- Helps reduce **revenue loss** due to churn

---

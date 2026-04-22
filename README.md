# Customer Churn Prediction using Machine Learning

##  Project Overview
This project investigates the use of machine learning models to predict customer churn in the telecommunications industry. The objective is to identify customers who are likely to leave a service provider and analyse how feature engineering and hyperparameter tuning affect model performance.

The models implemented in this project include:
- Logistic Regression
- Random Forest
- XGBoost

---

##  Research Question
Which machine learning models perform best in predicting customer churn using a real-world dataset, and how do feature engineering and hyperparameter optimisation influence their performance?

---

##  Dataset
The dataset used is the **IBM Telco Customer Churn Dataset**, which contains customer demographic, service usage, and billing information.

- Source: https://www.kaggle.com/datasets/blastchar/telco-customer-churn
- Records: 7,043 customers
- Target Variable: `Churn` (Yes/No)

---

##  Methodology

### Data Preprocessing
- Converted `TotalCharges` to numeric
- Handled missing values using median imputation
- Dropped irrelevant columns (e.g., `customerID`)
- One-hot encoded categorical variables
- Applied feature scaling for Logistic Regression

### Feature Engineering
- `AvgCharges`: Average monthly spend
- `TotalServices`: Number of subscribed services
- `HighSpender`: Indicator for high monthly charges
- `IsMonthlyContract`: Identifies high-risk contract type

### Models Used
- Logistic Regression (baseline)
- Random Forest (ensemble model)
- XGBoost (boosting model)

### Model Evaluation
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

### Validation & Tuning
- Stratified 5-Fold Cross-Validation
- GridSearchCV for hyperparameter tuning

---

## Results Summary
- Logistic Regression achieved the best overall performance
- Ensemble models did not significantly outperform the linear model
- Hyperparameter tuning provided minimal improvement
- Dataset shows relatively simple and near-linear patterns

---

## Visualisations
The project includes:
- Churn distribution plot
- Tenure vs churn analysis
- Monthly charges vs churn
- Contract type vs churn
- Model performance comparison
- ROC curves
- Confusion matrix

---

##  Key Insights
- Simpler models can outperform complex models in structured datasets
- Feature engineering improves interpretability and performance
- Class imbalance affects recall and model evaluation

---

##  Limitations
- Dataset is synthetic and may not reflect real-world complexity
- Moderate class imbalance affects performance
- Limited feature interactions

---

##  Future Work
- Apply advanced feature engineering techniques
- Use cost-sensitive learning for class imbalance
- Implement SHAP for explainability
- Test on larger and real-world datasets
- Explore deep learning models

---

##  Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

---

## 📂 Project Structure

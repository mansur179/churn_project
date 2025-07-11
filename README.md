# churn_project
A machine learning project to predict customer churn using Python and Scikit-learn.
# Proactive Customer Retention: Telco Churn Prediction

## 1. Business Problem
This project uses the standard Telco dataset to proactively identify customers who are at a high risk of "churning" (canceling their subscription). By predicting churn, a telecom company can focus its retention efforts on at-risk customers, thereby reducing revenue loss.

## 2. Results & Key Insights

*   **Performance:** The final model (XGBoost) achieved an **F1-Score of [0.83]** on the test set.
*   **Key Churn Drivers:** The most significant factors leading to customer churn were identified as:
    1.  **[Contract Type: Month-to-month]**
    2.  **[Tenure (how long they have been a customer)]**
    3.  **[Monthly Charges]**
*   **Recommendation:** The business should focus retention efforts specifically on customers identified by features 1 and 2.

## 3. Tech Stack
*   **Data Analysis:** Python, Pandas, NumPy
*   **Data Visualization:** Matplotlib, Seaborn
*   **Modeling & Evaluation:** Scikit-learn, [logisticregression,Random Forest,XGBoost]

## 4. The Process: From Data to Insights

1.  **Data Cleaning:** Processed the raw Telco data, handling missing values and encoding categorical features (like 'Contract Type' and 'Internet Service') using One-Hot Encoding.
2.  **Exploratory Data Analysis (EDA):** Analyzed the dataset to uncover initial insights. 
3.  **Modeling & Evaluation:** Trained and compared several classification models. The [XGBoost] model was selected due to its superior performance on the F1-metric (which is crucial for imbalanced datasets like churn).

## 5. How to Run This Project
The analysis and modeling can be reviewed in the `telco_project.ipynb` notebook. The dataset used is `WA_Fn-UseC_-Telco-Customer-Churn.csv`.

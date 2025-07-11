# Proactive Customer Retention: A Telco Churn Prediction Project

## 1. Business Problem
This project uses the standard Telco dataset to proactively identify customers who are at a high risk of "churning" (canceling their subscription). By predicting churn, a telecom company can focus its retention efforts on at-risk customers, thereby reducing revenue loss.

## 2. Results & Key Insights
*   **Performance:** The final XGBoost model achieved an **F1-Score of 0.83** on the test set, showing a strong capability to identify at-risk customers.
*   **Key Churn Drivers:** The most significant factors leading to customer churn were identified as:
    1.  Contract Type (specifically Month-to-month)
    2.  Tenure (how long they have been a customer)
    3.  Monthly Charges
*   **Recommendation:** The business should focus retention efforts on customers with short tenures on month-to-month contracts, as they represent the highest risk group.

## 3. Tech Stack
*   **Data Analysis:** Python, Pandas, NumPy
*   **Data Visualization:** Matplotlib, Seaborn
*   **Modeling & Evaluation:** Scikit-learn (Logistic Regression, Random Forest), XGBoost

## 4. The Process: From Data to Insights

1.  **Data Cleaning:** Processed the raw Telco data, handling missing values and encoding categorical features (like 'Contract Type' and 'Internet Service') using One-Hot Encoding.
2.  **Exploratory Data Analysis (EDA):** Analyzed the dataset to uncover initial insights.

3.  **Modeling & Evaluation:** Trained and compared several classification models. The XGBoost model was selected due to its superior performance on the F1-metric, which is crucial for imbalanced datasets like churn.

## 5. How to Run This Project
The analysis and modeling process can be reviewed in the `telco_project.ipynb` notebook. The dataset used is `WA_Fn-UseC_-Telco-Customer-Churn.csv`.

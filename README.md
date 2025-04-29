# Customer Churn Prediction

This project focuses on predicting customer churn for a telecommunications company. The goal is to identify customers who are likely to churn (leave the company) based on various features such as contract type, payment method, internet service, and more.

## Problem Statement

Customer churn is a critical issue for businesses, as retaining existing customers is more cost-effective than acquiring new ones. This project aims to develop a machine learning model to predict which customers are at risk of leaving, allowing the company to take proactive measures.

## Dataset

The dataset used in this project is publicly available and contains the following columns:

- `SeniorCitizen`: Whether the customer is a senior citizen (1 or 0).
- `tenure`: Number of months the customer has been with the company.
- `MonthlyCharges`: The amount the customer is billed monthly.
- `TotalCharges`: Total amount charged to the customer.
- `Churn`: Whether the customer has churned (Yes or No).
- `Contract`: Type of contract the customer has (e.g., month-to-month, one-year, two-year).
- `PaymentMethod`: The method by which the customer pays (e.g., electronic check, mailed check, credit card).
- **Other categorical variables**: such as `InternetService`, `TechSupport`, and `StreamingTV`, are also included.

## Objective

Predict whether a customer will churn based on features like `Contract`, `PaymentMethod`, `Tenure`, and `MonthlyCharges`.

## Approach

1. **Data Cleaning**: Handle missing values and encode categorical features.
2. **Exploratory Data Analysis**: Analyze the distribution of data and relationships between features.
3. **Feature Engineering**: Convert categorical variables to numerical representations using one-hot encoding.
4. **Model Building**:
    - **Logistic Regression**: A baseline model to predict churn.
    - **Random Forest Classifier**: An ensemble model to improve prediction accuracy.
5. **Evaluation**: The models were evaluated using accuracy, precision, recall, F1-score, and confusion matrix.

## Key Insights

- **Contract Type**: Customers with month-to-month contracts are more likely to churn.
- **Payment Method**: Customers paying via electronic check are more likely to churn.
- **Service Type**: Fiber optic customers tend to have a higher churn rate.
  
## Results

- **Logistic Regression** and **Random Forest** models gave comparable results in terms of accuracy.
- The models were able to predict churn with a reasonable degree of accuracy, providing valuable insights for business decision-making.

## Files

- `churn_prediction.ipynb`: Jupyter notebook containing the data analysis and machine learning model.
- `Customer_Churn.csv`: The dataset used for analysis.
- `churn_model.pkl`: The trained model, saved for future use.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Ka1lu/Customer-Churn.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebook to see the step-by-step analysis and model training.

## Conclusion

This project demonstrates how machine learning can be used to predict customer churn, which can help businesses identify at-risk customers and take action to retain them. The model can be further improved with additional features, hyperparameter tuning, or more advanced algorithms.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

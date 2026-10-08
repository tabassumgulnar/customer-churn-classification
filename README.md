# customer-churn-classification
Customer Churn Prediction using Logistic Regression | Machine Learning Internship Project
# Customer Churn Prediction using Logistic Regression

## Project Overview

This project is a Simple Classification Model developed as part of my Machine Learning Internship at CodeOrbit Tech.

The project focuses on predicting whether a customer is likely to churn (leave/cancel the service) using Logistic Regression.

## Objective

The main objectives of this project are:

- Preprocess customer churn data
- Convert categorical data into numerical form
- Split the dataset into training and testing sets
- Build a Logistic Regression classification model
- Evaluate the model using Accuracy, Precision, and Recall

## Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains customer information such as:

- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure
- Internet Service
- Contract
- Payment Method
- Monthly Charges
- Total Charges
- Churn

The target variable is `Churn`.

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Converted `TotalCharges` into numerical format.
3. Handled missing values using the median.
4. Removed the `customerID` column.
5. Converted categorical variables into numerical features using one-hot encoding.

## Model

The classification model used in this project is:

**Logistic Regression**

The dataset was divided into:

- Training data: 5,634 records
- Testing data: 1,409 records
- Features used: 30

## Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall

### Results

| Metric | Score |
|---|---:|
| Accuracy | 82.11% |
| Precision | 68.50% |
| Recall | 60.05% |

## Results Interpretation

The model achieved an accuracy of 82.11%, meaning it correctly classified around 82% of the test records.

The precision for churn prediction was 68.50%, meaning that among the customers predicted as likely to churn, about 69% actually churned.

The recall was 60.05%, meaning the model identified around 60% of the customers who actually churned.

The model performed better at identifying customers who stayed than customers who churned, so there is room for improving churn detection.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab
- Jupyter Notebook

## Project Files

- `Simple_Classification_Model_Customer_Churn_Final.ipynb` — Complete Google Colab/Jupyter Notebook
- `Customer_Churn_Classification_Model_Report.pdf` — Project report

## Conclusion

This project demonstrates how a simple classification model can be used to predict customer churn. Logistic Regression provided a good baseline performance with 82.11% accuracy.

## Future Scope

The model can be improved in the future by:

- Trying other classification algorithms
- Hyperparameter tuning
- Improving recall for churned customers
- Using additional feature engineering techniques

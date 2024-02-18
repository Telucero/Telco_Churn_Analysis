# Telco - Churn Rate: Predicting Customer Churn
## Introduction
Welcome to the Telco Churn Rate analysis! In this project, I aim to predict customer churn for Telco, a telecommunications company. Customer churn refers to the rate at which customers leave the service, canceling their subscription. By utilizing predictive analytics, Telco can identify potential churners based on customer attributes, allowing them to implement targeted strategies such as promotions or customer experience improvements.

## Dataset Overview
The dataset comprises 7043 instances with 21 variables. Here's a brief overview of the key variables:

CustomerID: Unique customer identifier
Gender: Male or Female
Senior Citizen: Binary indicator of senior citizen status (0 or 1)
Partner: Marriage status (Yes or No)
Dependents: Dependents status (Yes or No)
Tenure: Number of years with Telco
Phone Service: Phone service status (Yes or No)
Multiple Lines: Multiple lines setup status (Yes, No, or No Phone Service)
Internet Service: Internet service status (DSL, Fiber Optic, or No)
Online Security: Online security provision status (Yes, No, or No Internet Service)
Online Backup: Online backup provision status (Yes, No, or No Internet Service)
Device Protection: Device protection provision status (Yes, No, or No Internet Service)
Tech Support: Tech support provision status (Yes, No, or No Internet Service)
Streaming TV: Streaming TV provision status (Yes, No, or No Internet Service)
Streaming Movies: Streaming movies provision status (Yes, No, or No Internet Service)
Contract: Contract type (Month-to-Month, One Year, or Two Year)
Paperless Billing: Billing method (Yes or No)
Payment Method: Payment method (Bank Transfer, Mailed Check, Credit Card, or E-Check)
Monthly Charges: Monthly charge amount
Total Charges: Total charge amount over time
Churn (Target Variable): Churn status (Yes or No)

## Simple Analysis Overview
The analysis consists of the following steps:

Data Preprocessing: Cleaned the dataset to handle missing values.
Variable Conversion: Converted categorical variables into numeric factor forms for modeling purposes.
Model Building: Constructed predictive models using the Decision Tree algorithm.
Evaluation: Evaluated model performance using confusion matrices and key performance metrics such as precision, recall, accuracy, and F1-measure.
Model Refinement: Tuned hyperparameters to improve model performance and mitigate overfitting or underfitting.
Results and Impact Explanation
The analysis provided valuable insights into Telco's customer churn dynamics and its impact on business decisions:

## Model Performance:

The initial model achieved an accuracy of 80%, indicating that it correctly classified 80% of the customers.
Precision, which measures the proportion of correctly predicted positive cases among all predicted positive cases, was 94%. This suggests that 94% of the customers predicted to churn actually did churn.
Recall, also known as sensitivity, was 83%, indicating that the model correctly identified 83% of the actual churn cases.
The F1-measure, which considers both precision and recall, was 88%.

## Variables Importance:

By analyzing the beta coefficients and t-values, we identified variables that were not statistically significant in predicting churn. These included Gender, Streaming TV, Streaming Movies, and Payment Method. Removing these variables improved model performance and reduced complexity.

## Model Refinement:

Tuning hyperparameters helped refine the model and improve its predictive capabilities. Pruning the decision tree led to a slight reduction in false negatives, enhancing the model's ability to identify customers at risk of churn.

## Business Impact:

The predictive models provide Telco with actionable insights to retain customers and enhance customer satisfaction.
By targeting potential churners with personalized promotions or improved customer service, Telco can reduce customer churn and increase revenue.
The analysis highlights the importance of continuous monitoring and refinement of predictive models to adapt to changing business conditions and customer behaviors.
Packages Used
readr
lm.beta
rpart
rpart.plot
e1071
caret
yardstick
Feel free to explore the provided code and analysis to gain deeper insights into Telco's customer churn dynamics.

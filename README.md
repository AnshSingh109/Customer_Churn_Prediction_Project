# Customer_Churn_Prediction_Project
Customer Churn Prediction using Random Forest, KNN, Naive Bayes 

Customer retention is one of the most critical challenges faced by businesses, especially in competitive industries like telecommunications. Understanding the factors that lead customers to discontinue their services—commonly known as customer churn—is essential for maintaining profitability and growth. This project focuses on predicting customer churn using machine learning techniques applied to a publicly available telecom customer dataset.

We will perform:

Exploratory Data Analysis (EDA): to understand data patterns, distributions, and correlations.

Feature Scaling: to normalize numerical values for better model performance.

Evaluation Metrics: to assess model performance and accuracy

Customer retention is one of the most critical challenges faced by businesses, especially in competitive industries like telecommunications. Understanding the factors that lead customers to discontinue their services—commonly known as customer churn—is essential for maintaining profitability and growth. This project focuses on predicting customer churn using machine learning techniques applied to a publicly available telecom customer dataset.

We will perform:

Exploratory Data Analysis (EDA): to understand data patterns, distributions, and correlations.

Feature Scaling: to normalize numerical values for better model performance.

Evaluation Metrics: to assess model performance and accuracy

## ML Algorithms Used

### Random Forest

Random Forest is an ensemble learning algorithm that builds multiple decision trees and combines their outputs to make a final prediction.
Each tree learns from a random subset of the data, and the final prediction is based on majority voting.

Why it's effective:

- Reduces overfitting

- Handles both numerical & categorical data

- Gives high accuracy and feature importance

### K-Nearest Neighbors (KNN)

KNN is a distance-based algorithm that classifies a new data point based on the K closest neighbors in the feature space.
It assumes that similar data points tend to belong to the same class.

Why it's effective:

- Simple and intuitive

- Works well with properly scaled data

- No training time — all computation happens during prediction
<br>

### Naive Bayes

Naive Bayes is a probabilistic algorithm based on Bayes’ Theorem.
It calculates the probability of each class given the input features and predicts the class with the highest probability.
It is called “naive” because it assumes all features are independent.

Why it's effective:

- Fast and efficient

- Works well with large and high-dimensional data

- Often used in text classification & spam detection

- Customer churn is one of the most significant challenges faced by the telecom industry. As competition increases, retaining existing customers becomes far more cost-effective than acquiring new ones. Predicting which customers are likely to leave the service enables companies to take proactive retention actions, design targeted offers, and enhance overall customer satisfaction.

The Telco Customer Churn dataset contains detailed information about each customer, including demographic factors, service subscriptions, account details, billing methods, and monthly spending patterns. Key attributes such as tenure, contract type, internet service, payment method, monthly charges, and churn status provide valuable insights into customer behavior and potential risk factors that may contribute to churn.

The objective of this project is to explore and analyze these features through data preprocessing and exploratory analysis, then apply machine learning techniques to build accurate churn prediction models. By classifying customers into “Churn” and “Not Churn,” the system can help telecom companies understand churn drivers, reduce customer loss, and make data-driven business decisions.

### Heatmap: Correlation Between Numerical Features

A correlation heatmap helps identify how numerical features in the dataset are related to each other. In customer churn analysis, understanding these relationships is important because certain patterns—such as higher charges or longer tenure—may influence a customer’s likelihood of leaving the service. By visualizing correlations, we can easily detect strong positive or negative relationships among features like MonthlyCharges, TotalCharges, tenure, and SeniorCitizen, which helps us better understand customer behavior and guides feature selection for machine learning models.

<img width="625" height="528" alt="image" src="https://github.com/user-attachments/assets/58db6257-0442-4bf7-83f8-2e75fd080cca" />



#### 5. Confusion Matrix

**Definition**:

A Confusion Matrix is a 2×2 table that summarizes the model’s predictions by comparing them with the actual class labels.
It shows how many customers were correctly or incorrectly classified as Churn or Not Churn.
<br><br>

**Matrix Structure**

|                 | **Predicted: No**   | **Predicted: Yes**  |
| --------------- | ------------------- | ------------------- |
| **Actual: No**  | True Negative (TN)  | False Positive (FP) |
| **Actual: Yes** | False Negative (FN) | True Positive (TP)  |

<br>

**Purpose**:

- Helps understand exactly where the model is making mistakes

- Shows types of errors:

   - False Positives (FP) → model predicts churn, but customer stays

   -  False Negatives (FN) → model predicts no churn, but customer actually churns (most critical)

- Helps interpret Precision, Recall, and F1-Score

- Provides a clear visual breakdown of model performance beyond accuracy


<img width="444" height="393" alt="image" src="https://github.com/user-attachments/assets/0e4a813c-682e-4d10-a64b-a00fed870a0a" />


### Feature Importance (Random Forest)

Feature importance helps us understand which features contribute the most to the model's predictions.
Random Forest provides built-in feature importance by measuring how much each feature improves the model’s performance when used for splitting decision trees.

In this project, the following steps were done:

Extracted feature importance from the trained Random Forest model

Sorted and selected the top 10 most important features

Plotted a horizontal bar chart for easy visualization

This graph shows which factors have the strongest impact on predicting customer churn.
Features like tenure, monthly charges, contract type, and total charges usually appear as the most influential in churn prediction.


<img width="883" height="451" alt="image" src="https://github.com/user-attachments/assets/9dc53464-2390-44b7-b7d5-8774ed93300a" />

### Step - 8: Visualization of Predictions


A line graph comparing the actual and predicted churn values helps visualize how closely each model’s predictions match the true customer outcomes. By plotting all three models together, we can easily observe which algorithm follows the actual churn pattern more accurately. This comparison provides a clear and intuitive understanding of model performance over the same set of customers.


<img width="549" height="374" alt="image" src="https://github.com/user-attachments/assets/1e1e46ed-1bc8-41aa-92b1-3a1325c712df" />


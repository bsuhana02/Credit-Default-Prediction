# Credit-Default-Prediction

**Problem Statement** : 
Financial threats are increasingly posing challenges to the credit risk assessment of commercial banks, particularly due to significant advancements in the financial industry. One of the most pressing threats faced by these banks is accurately predicting the credit risk of clients. This project aims to predict the probability of credit default based on the characteristics of credit card owners and their payment history.

**Approach**
To tackle the problem of credit default prediction, we will employ a systematic machine learning workflow comprising several key tasks:

**1. Data Exploration** : 
Investigate the dataset to understand its structure, identify data types, and uncover initial insights.
Visualize distributions, relationships, and trends within the data using graphs and statistical measures.

**2. Data Cleaning** :
Handle missing values through imputation or removal based on their significance and impact.
Detect and correct inconsistencies or anomalies within the dataset to ensure data integrity.

**3. Feature Engineering** :
Create new features that could enhance model performance, such as aggregating payment histories or encoding categorical variables.
Select relevant features that contribute significantly to predicting credit defaults while eliminating redundant or irrelevant ones.

**4. Model Building** :
Experiment with various classical machine learning algorithms to determine which models best fit the data. Potential algorithms to consider include:
Logistic Regression: A statistical model suitable for binary classification.
Decision Trees: A non-linear model that makes decisions based on feature values.
Random Forest: An ensemble method that utilizes multiple decision trees to improve accuracy and robustness.
Gradient Boosting Machines (GBM): A powerful ensemble technique that builds models in a stage-wise manner to optimize prediction accuracy.
Support Vector Machines (SVM): A model that identifies the hyperplane that best separates classes in the feature space.

**5. Model Testing** :
Evaluate the performance of the models using appropriate metrics such as accuracy, precision, recall, F1-score, and area under the ROC curve (AUC-ROC).
Utilize cross-validation techniques to ensure the models generalize well to unseen data.

# Results
The ultimate goal of this project is to develop a robust solution capable of predicting the probability of credit default based on the characteristics and payment histories of credit card owners. The performance of the models will be assessed through rigorous testing, and insights will be derived to help improve credit risk management strategies for commercial banks. By achieving this, the project aims to contribute to reducing financial risks and enhancing the stability of the banking sector.

# Dataset Description: 
The dataset is related to a credit card default prediction task, where the goal is to predict whether a credit card holder will default on their payment in the next month. It contains various features related to the individual’s personal information, credit history, payment history, and bill amounts. The target variable is whether the individual defaults on the payment in the subsequent month.
Each row represents an individual with information about their credit card usage, payment history, personal details, and whether or not they defaulted on their payment in the next month. Here's an explanation of the columns:
**Column Descriptions:**

ID:
Type: Numeric
A unique identifier for each individual in the dataset.

LIMIT_BAL:
Type: Numeric
The credit limit given to the individual on their credit card.

SEX:
Type: Categorical (1, 2)
The gender of the individual (1 = male, 2 = female).

EDUCATION:
Type: Categorical (1, 2, 3, 4)
The education level of the individual:
1 = Graduate school
2 = University
3 = High school
4 = Others

MARRIAGE:
Type: Categorical (1, 2, 3)
The marital status of the individual:
1 = Married
2 = Single
3 = Others

AGE:
Type: Numeric
The age of the individual.

PAY_1 to PAY_6:
Type: Numeric (with values ranging from -2 to 2)
These columns represent the payment status for the past 6 months. A negative number indicates a delay in payment:
0 = No delay (on time)
-1 = Payment delay for 1 month
-2 = Payment delay for 2 months
-3 = Payment delay for 3 or more months
1, 2 are also possible (indicating 1 or 2 months overdue payments).

BILL_AMT1 to BILL_AMT6:
Type: Numeric
These columns represent the bill statement amounts for the past 6 months. They reflect how much was owed by the individual in each month.

PAY_AMT1 to PAY_AMT6:
Type: Numeric
These columns represent the payments made by the individual over the past 6 months. They show how much the individual paid towards their bills in each month.

default.payment.next.month:
Type: Categorical (0, 1)
This is the target variable that indicates whether the individual defaulted on their payment in the next month:
1 = Default
0 = No default

# Summary of the Dataset
Target Variable: default.payment.next.month (the prediction target).
Features: Various demographic, credit, and payment history data, including age, gender, education, marital status, payment history, bill amounts, and payment amounts over the last 6 months.
Use Case: The dataset is used to predict whether an individual will default on their credit card payment in the next month. It can be used for training machine learning models, such as logistic regression, decision trees, or more advanced models like neural networks, to predict the likelihood of default based on the individual’s financial history.

The goal in this dataset is typically to predict whether a person will default on their credit payment in the next month (default.payment.next.month) based on the other variables, such as payment history, credit limit, age, and so on.


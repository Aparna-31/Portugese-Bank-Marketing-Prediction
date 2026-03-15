Bank Marketing Campaign Analysis & Subscription Prediction
Project Overview

Marketing campaigns are a key strategy used by banks to promote financial products such as term deposits. However, large-scale campaigns often involve contacting thousands of customers, which can be expensive and inefficient if not properly targeted.

This project analyzes the Portuguese Bank Marketing Dataset and develops a machine learning model to predict whether a customer will subscribe to a term deposit. The goal is to help the bank identify high-potential customers, improve campaign efficiency, and reduce marketing costs through data-driven decision-making


Business Problem

Banks frequently conduct direct marketing campaigns via phone calls to promote term deposit products. However:

Contacting all customers leads to high operational costs.

Many contacted customers do not subscribe.

Potential customers may be missed due to poor targeting.

This project aims to solve this problem by building a predictive model that identifies customers who are more likely to subscribe, enabling smarter marketing strategies.

Target Variable

y

1 → Customer subscribed to term deposit

0 → Customer did not subscribe


Project Workflow
1. Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand:

Customer demographics

Campaign performance

Feature distributions

Correlations between variables

Class imbalance in the dataset

Key visualizations were used to identify patterns and trends in customer behavior.

2. Data Preprocessing

The following preprocessing steps were performed:

Handling categorical variables using encoding techniques

Feature scaling where necessary

Splitting dataset into training and testing sets

Addressing class imbalance considerations


3. Model Development

A Logistic Regression classifier was implemented to predict whether a customer will subscribe to the term deposit.

Logistic Regression was chosen because:

It is effective for binary classification problems

It provides interpretable probability outputs

It performs well for marketing response prediction

Model Performance
Accuracy

81.86%

Classification Report
Class	Precision	Recall	F1 Score	Support
Not Subscribed (0)	0.95	0.84	0.89	7265
Subscribed (1)	0.35	0.63	0.45	971
Confusion Matrix
	Predicted No	Predicted Yes
Actual No	6127	1138
Actual Yes	356	615
Model Evaluation Insights

In marketing prediction problems, Recall is a critical metric.

A False Negative occurs when the model predicts a customer will not subscribe, but the customer would actually subscribe.

This results in lost revenue opportunities, making recall particularly important.

At the same time, Precision must also be considered, because:

Low precision means contacting many uninterested customers

This increases marketing costs and operational workload

Therefore, the selected model balances recall and precision to support effective marketing decisions.

Key Business Insights

The analysis reveals several important patterns:

Customers who responded positively in previous campaigns are more likely to subscribe again.

Targeted marketing is significantly more effective than mass outreach campaigns.

Customer profile characteristics can strongly influence subscription probability.

Data-driven strategies can help optimize marketing efficiency and cost management.

Strategic Recommendations for the Marketing Team

Based on the model predictions and data analysis:

Prioritize contacting customers with higher predicted subscription probability.

Reduce calls to customers with low likelihood of subscribing to save marketing costs.

Use personalized marketing strategies based on customer profiles.

Focus on customers with positive responses in previous campaigns.

Use phone calls for high-probability customers and alternative channels such as SMS or email for others.

Avoid repeated calls that may lead to customer dissatisfaction.

Continuously update the predictive model using new campaign data.

Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

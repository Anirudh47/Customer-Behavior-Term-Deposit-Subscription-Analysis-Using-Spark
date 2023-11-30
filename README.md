# BAN5753_Team_Incisive_MiniProject_2

## Introduction
XYZ Bank seeks to optimize its direct marketing campaigns for term deposit subscriptions. By applying machine learning models, the bank aims to predict which customers are more likely to subscribe, thus improving the allocation of marketing resources and customer engagement strategies.

## Problem Statement
The primary objective of this project is to classify clients based on their propensity to subscribe to a term deposit. This involves analyzing various client attributes and their interaction with the bank's marketing campaigns. The classification task is binary: predicting whether a client will subscribe ('yes') or not ('no') to a term deposit. A key element of this project is Exploratory Data Analysis (EDA), which aims to uncover patterns, relationships, and trends within the data, providing valuable insights into factors influencing client decisions.

## Dataset
The dataset, "XYZ_Bank_Deposit_Data_Classification.csv", encompasses records from May 2008 to November 2010, detailing the bank's direct marketing campaigns conducted via telephone calls. It comprises 20 attributes, including:
Age: Numeric
Job: Categorical (type of job)
Marital Status: Categorical
Education: Categorical
Default: Categorical (credit in default)
Housing: Categorical (housing loan)
Loan: Categorical (personal loan)
Contact: Categorical (type of contact communication)
Month: Categorical (last contact month)
Day of Week: Categorical (last contact day)
Duration: Numeric (last contact duration in seconds)
Campaign: Numeric (contacts during the current campaign)
Pdays: Numeric (days since last contact in previous campaign)
Previous: Numeric (contacts before current campaign)
Poutcome: Categorical (outcome of previous campaign)
Emp.var.rate: Numeric (employment variation rate)
Cons.price.idx: Numeric (consumer price index)
Cons.conf.idx: Numeric (consumer confidence index)
Euribor3m: Numeric (euribor 3 month rate)
Nr.employed: Numeric (number of employees)

## Exploratory Data Analysis (EDA)
The EDA involved creating histograms and a correlation heatmap for numerical features. Key findings include a concentration of clients aged 30-40, most not contacted before (pdays at 999), and a right-skewed distribution in call durations. The correlation heatmap highlights a moderate positive correlation between the number of employees and employment variation rate, and a strong positive correlation between the Euribor 3-month rate, number of employees, and employment variation rate.

## Model Development and Evaluation**
We implemented several machine learning models, each evaluated by the Area Under the ROC Curve (AUC).
Decision Tree Classifier
AUC: 0.6704
The model is relatively simple and fast but less powerful.
Random Forest Classifier
AUC: 0.9312
An ensemble method that provided better generalization than the Decision Tree.
Gradient Boosting (GBT) Classifier
AUC: 0.9463
This model performed the best among the classifiers and will be chosen for deployment.


## K-means Clustering Analysis
Optional clustering was performed to identify distinct groups within the clients based on numerical features.
Clustering could inform targeted marketing strategies by identifying segments with higher likelihoods of subscription.

## Visualization and Clustering
Visualizations from the K-means clustering reveal distinct groupings in the dataset:
Age vs. Euribor 3m Rate: Indicates potential clusters based on age and prevailing interest rates.
Campaign vs. Duration: Shows groupings based on the number of contacts during a campaign and the call duration.
Employment Variation Rate vs. Consumer Price Index: May suggest economic clusters that could influence a client's decision.
Consumer Confidence Index vs. Number of Employees: Could provide insights into market sentiments and employment trends.
These visual insights can guide the bank in understanding customer profiles and the economic factors affecting their decisions.


## Results and Recommendations
The Gradient Boosting Classifier is the recommended model for deployment due to its superior performance. The clustering analysis provides additional insights and could be used for market segmentation. The bank should consider these models and analyses to refine its marketing strategies and potentially increase the subscription rate.


 ## Objective
The Analysis in XYZ Bank's marketing strategy empower the bank to uncover patterns, understand customer behavior, and efficiently target individuals with a higher likelihood of subscribing to a term deposit. This data-driven approach enhances the effectiveness of the marketing campaign, ultimately leading to increased success in attracting new term deposit customers.



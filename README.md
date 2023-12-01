# Customer churn analysis

![logo](https://github.com/mumbikariuki/Phase4-project/blob/main/logo/2011-634524812437378998-737.jpg)

# Overview
 This project involves a data analysis that focuses on determining what features will indicate if a customer will ("soon") discontinue their service.
    
# Target audience
This data is more importantly of interest to various stakeholders that  play critical roles in the project. These stakeholders include:      a)Syria Tel company at large :This also involves the company's executives, shareholders and investors.
b)Customers are indirectly impacted. The goal is to improve services and customer satisfaction, potentially reducing churn and ensuring a positive experience for existing customers.
C)Customer Service Teams  who benefit from understanding patterns indicative of potential churn. This information enables them to proactively engage with customers, address concerns, and enhance the overall customer experience.

# Business understanding
# Introduction

In the dynamic landscape of the telecommunications industry, SyriaTel is facing the challenge of customer churn, which directly impacts its revenue and market share. The company recognizes the need for a proactive approach to identify and retain customers who are likely to discontinue their services in the near future. The objective is to develop a robust predictive model that accurately anticipates customer churn based on historical data and behavioral patterns. 

# Problem statement
The telecommunications industry is marked by intense competition, making customer retention a critical factor for sustained profitability. SyriaTel seeks to proactively address customer churn by leveraging predictive analysis on historical customer data. This project aims to develop a robust model that can accurately identify customers at risk of churn, enabling SyriaTel to implement targeted retention strategies.

# Objectives
### Main objective
The primary goal is to develop a binary classification model that accurately predicts whether a customer is likely to churn ("soon") or not.

### Other objectives
Explore and utilize historical customer data to identify patterns and behaviors indicative of potential churn.
Evaluate and compare the performance of various classification algorithms to select the most effective model for SyriaTel's specific context.
Turn Data Results into Practical Advice for SyriaTel:Translate the computer results into practical advice that SyriaTel can use.

# Data understanding
The dataset used for this analysis comprises historical customer data, including features such as call duration, data usage, contract length, customer service interactions, and more. The target variable is binary, indicating whether a customer has churned or not.

# Results and interpretation
## Baseline model
Using logistic regression as a baseline model typically involves applying a simple and interpretable algorithm to establish a starting point for comparison with more complex models.
The accuracy score of 85.16% in the logistic regression model  represents the proportion of correctly classified instances among the total instances. In this case, 85.16% of predictions were correct.The accuracy is relatively high but on the contrary, for class 1 (churn happening), the precision is lower, indicating that the model has more false positives thus suggests that the model misses a significant portion of actual churn instances.
This suggests that there is room for improvement.

## Random Forest Classifier
The Random Forest classifier shows a significant improvement in accuracy compared to the logistic regression model by having an accuracy s score of 95% which i spretty good.
Precision, Recall, and F1-Score for both classes have improved, indicating a better balance between correctly identifying instances of class 1 (churning)and avoiding false positives.The model excels in predicting class 0(not churning) , with very high precision and recall.
After tuning the hyperparameters in this model in order to optimize it, it increased its accuracy score to 96% suggesting that  when using a specific threshold for classification decisions, the model is accurate in predicting the correct class for about 96.10% of the instances.

## Ensemble method(XGBOOST)
XGBClassifier yielded an  accuracy score of 95% is pretty good but it did not perform better compared our Random Forest Classifier that used tuned hyper parameters.

# Conclusion
The Random Forest Classifier  model excels with the highest accuracy score of 96.10% outperforming the baseline and the ensemble method.This results collectively demonstrate the Random Forest model's stronger performance in predicting rhe outcome of whether a customer will churn or not.
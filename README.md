# SyriaTel Customer Churn Prediction

## Project Overview

This project focuses on predicting customer churn for SyriaTel, a telecommunications company. Customer churn refers to customers who stop using the company's services.

The objective is to build a machine learning model that can identify customers likely to churn, enabling the business to take proactive measures to retain them.

## Dataset Description

The dataset contains 3,333 customer records with 21 features, including:

* Customer demographics (state, account length)
* Service plans (international plan, voicemail plan)
* Usage patterns (call minutes, charges)
* Customer service interactions

Target variable:

* `churn` (1 = churn, 0 = stay)

## Data Preparation

* Dropped irrelevant columns (phone number)
* Converted categorical variables to numeric
* One-hot encoded categorical features (state)
* Verified all data types were suitable for modeling

## Exploratory Data Analysis

Key findings:

* Churn rate is approximately 14–15%
* Customers with more customer service calls are more likely to churn
* High usage and charges are associated with higher churn
* International plan users show higher churn rates

## Models Used

* Logistic Regression
* Random Forest

## Model Evaluation

Performance was evaluated using:

* Accuracy
* Precision
* Recall (primary focus)
* F1-score

## Model Optimization

Hyperparameter tuning was performed using RandomizedSearchCV to improve model performance.

The tuning focused on maximizing recall to ensure more churners are correctly identified.

## Final Model

The tuned Random Forest model was selected as the best model.

### Performance:

* Accuracy: 89%
* Recall (churn): 76%
* Precision (churn): 58%

## Key Insights

* Customer service calls are the strongest indicator of churn
* High usage customers are more likely to leave
* Pricing and service experience significantly influence customer retention

## Business Recommendations

* Implement churn prediction system
* Improve customer support services
* Offer personalized pricing plans
* Proactively engage high-risk customers

## Conclusion

The project demonstrates that machine learning can effectively predict customer churn and provide actionable insights to improve customer retention.


## Technologies Used

* Python
* Pandas
* Scikit-learn
* Matplotlib / Seaborn

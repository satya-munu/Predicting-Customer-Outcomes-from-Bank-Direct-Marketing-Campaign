# Predicting-Customer-Outcomes-from-Bank-Direct-Marketing-Campaign
I developed a predictive model that targets 80% of potential customers by leveraging the top 46.4% of predictions. The classification goal is to predict if the client will subscribe to a term deposit. 
![Marketing Lift.png](https://raw.githubusercontent.com/satya-munu/Predicting-Customer-Outcomes-from-Bank-Direct-Marketing-Campaign/refs/heads/main/Marketing%20Lift.png)

## Data Overview
The data is from a Portuguese retail bank (2008-2013). To account for costs and the severity of false negatives over false positives, all models are trained with weights to place more emphasis on not missing potential customers. Additionally, the duration of the call, which is a feature that is only known after an agent calls a customer, is dropped from the dataset to avoid data leakage. 


## Model Comparison
Here are the models I created. Although CatBoost was the best-performing model with 80% accuracy, false negatives, or missing potential customers, is more consequential in a marketing context. Therefore, I would consider using the Random Forest model, which has the lowest false negative rate.
![Bank Marketing Model.png](https://raw.githubusercontent.com/satya-munu/Predicting-Customer-Outcomes-from-Bank-Direct-Marketing-Campaign/refs/heads/main/Bank%20Marketing%20Model.png)

## Recommendations
The key indicators of customers likely to subscribe to the term deposit include communication methods, the time of year the customer was last contacted, the outcome of the previous campaign, and bank balance. 
![Feature Importances.png](https://raw.githubusercontent.com/satya-munu/Predicting-Customer-Outcomes-from-Bank-Direct-Marketing-Campaign/refs/heads/main/Feature%20Importance.png)

Since having a housing loan is also important, the Bank could focus on targeting customers who responded positively to the last campaign and have longer-term investments with the bank, like a housing loan. 

Additionally, basic demographic characteristics, like age, marital status, occupation, and education, could be considered a cluster of the second most important features. The Bank could consider segmenting based on these attributes to develop a more targeted approach to identifying customers likely to subscribe to a term deposit. 

Data Source: Moro, S., Rita, P., & Cortez, P. (2014). Bank Marketing [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5K306.



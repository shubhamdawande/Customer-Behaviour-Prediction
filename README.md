# Customer-Behaviour-Prediction
Customer Segmentation for Marketing, RFM Analysis, Purchase Day Prediction

### Problem Statement:
We help Rainbow Store understand and predict customer behaviours. Here we are dealing with store’s basket-level transaction data. The store manager wants to know which customers are likely to purchase next month so he can prepare his marketing campaign.

1. Implement a model that predicts which customers make at least 1 purchase in a given month using features generated from the 2 previous months.
For example, data from February and March can be used to predict purchases in April; data from March and April can be used to predict purchases in May.

2. You're asked which customers to send promotional e-mails to next month, based on your model. What is your recommendation?


### Data:

- csn, date, salesqty, price/unit, article_id
- We have total of 5 months of txn data


### Feature Engineering:
- RFM
- Customer Segments Calculated using Cluster Analysis
- Last 5 purchase days per customer
- Distribution (mean, std) of purchase day difference
- Target label: Purchase day in given month

### Modelling:
- XGBoost (Final Model)
- K-fold Cross Validation

### Evaluation:
- Accuracy
- Train: 83%, Test: 78%

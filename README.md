# Bank_Dataset_Machine_Learning_Project

### Information
The data is related to direct marketing campaign direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.
bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]
The smallest datasets are provided to test more computationally demanding machine learning algorithms (e.g., SVM). 

### Main Task

The task is to build a model to predict whether a customer will open a term deposit at a bank. We encounter similar tasks in various companies and domains when we want to understand whether a customer will buy a certain product, use our service/website next month, or purchase a subscription.
Therefore, it is not enough to simply build a model; we must also explain how this model works and why it produces these specific results. Without this understanding, the client will not be able to proceed to deploying the model in production.

The classification goal is to predict if the client will subscribe a term deposit (variable y).

For this task, I am using a dataset that was originally published on the [UCI Machine Learning Repository] website; however, since that site provides an inaccurate description of the data and contains many different subsets, I decided to use the dataset from Kaggle: https://www.kaggle.com/datasets/sahistapatel96/bankadditionalfullcsv.

## 📊 Results

We compare the performance of different machine learning models based on key evaluation metrics.

| 🤖 Model            | 📈 Train ROC-AUC | 📉 Test ROC-AUC | 🔁 Train F1 | 🔁 Test F1 | 🎯 Train Recall | 🎯 Test Recall | 🎯 Train Precision | 🎯 Test Precision |
|--------------------|------------------|-----------------|-------------|------------|----------------|----------------|-------------------|------------------|
| Logistic Regression | 0.79             | 0.80            | 0.45        | 0.46       | 0.63           | 0.65           | 0.35              | 0.36             |
| kNN                | 0.92             | 0.74            | 0.48        | 0.38       | 0.29           | 0.29           | 0.56              | 0.56             |
| Decision Tree      | 0.83             | 0.77            | 0.51        | 0.48       | 0.73           | 0.61           | 0.38              | 0.40             |
| XGBoost            | 0.84             | 0.81            | 0.43        | 0.38       | 0.64           | 0.27           | 0.36              | 0.67             |

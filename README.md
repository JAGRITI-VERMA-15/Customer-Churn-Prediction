# Customer-Churn-Prediction

- **Name** - Jagriti
- **Project** - Customer Churn Prediction
- **Tools** -  Jupyter Notebook , Python , Numpy , Pandas , Matplotlib , Seaborn , Sklearn
- **Algorithms Used** - Decision Tree , Random Forest , Logistic Regression , XGBoost , GridSearchCV 
- **Evaluation Metrics** - GridSearchCV , Cross-Validation , Confusion Matrix , classificatiob report , ROC-AUC curve , Precision, Recall, F1-score  

# Business Understanding : 

A major telecom company is losing subscribers every month, which impacts its revenue and profitability. Predicting which customers are likely to churn helps to retain them through targeted offers and interventions.

# Problem Statement : 

Currently, the company lacks a proactive approach—customers at risk of leaving aren’t identified early, leading to reactive retention and inefficient spending. Analyzing usage and demographics can reveal churn patterns, enabling timely and focused retention efforts.

# Project Overview :

This project aims to identify customers which are at risk of churning by building a predictive model using demographic data. The model enables the business to:
- Detect high-risk customers before they leave  
- Understand the key factors driving churn  

# Dataset : 

The data was taken from Kaggle site : https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data

# Project Overflow :

Here is brief overview what i did :
- Firstly I explored the dataset to understand available features.
- Then, I perform Data cleaning by removing null entries, corrected data types, and dropped irrelevant columns to ensure data integrity.
- After that, I performed EDA including:
  - Univariate analysis for feature distributions and value counts.  
  - Bivariate analysis (e.g., churn vs. tenure, monthly charges vs. churn) to uncover key patterns.
- Then I encoded categorical variables and transformed the dataset for training.

### Model Training 

- Before training models, i performed train test split to evaluate model performance properly.
- Then train data using models- Logistic Regression, Random Forest, XGBoost and Decision Tree.
- Used **GridSearchCV** for each model to tune hyperparameters via cross-validation and select optimal configurations.

### Model Evaluation

- Evaluated each tuned model using key metrics: accuracy, precision, recall, F1‑score, cross validation and ROC‑AUC score.
- Compared model performance and selected the best-performing model based on a balanced trade-off of precision, recall, and AUC.

# Conclusion

The **XGBoost Classifier** was selected as the final model because it achieved the best overall performance:

- **Accuracy**: 74.0%  
- **Recall (Churn class)**: 80%  
- **F1-Score (Churn class)**: 0.62  
- **ROC-AUC**: **0.76** (highest among all models)  
- **Cross-validation score**: 75.41% (consistent generalization performance)

These results indicate that XGBoost is not only good at detecting churners (high recall) but also avoids many false alarms (reasonable precision), making it the most balanced and reliable model for this task.







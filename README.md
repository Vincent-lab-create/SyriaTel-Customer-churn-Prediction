# SyriaTel-Customer-churn-Prediction
# Project Overview
This project aims to help SyriaTel, a telecommunications company, reduce revenue loss by predicting which customers are likely to stop using their services soon. By analyzing customer data, we explore whether there are predictable patterns in customer behavior that signal impending churn.

# Business Understanding
Customer churn is a critical challenge in the telecommunication industry and SyriaTel is no exception. High churn rates directly translate to lost revenue, reduced profitability and high customer acquisition costs. My primary goal is to come up with a classifier that will predict whether a customer will stop using SyriaTel's services.

# Key Business Questions
- How does customer service interaction quality impact churn?
- Are customers on flexible or prepaid plans more prone to churn compared to those on fixed contracts?
- How do external market factors (e.g., competitor promotions, pricing wars) correlate with churn?
- Do demographic factors like age, gender, or occupation correlate with churn risk?

# Data Understanding
The dataset I used find it [Here](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset)

# Tech Stack
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn

# EDA
* 1 Top 10 states with highest churn

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/6a7e2b1e4c86b42897798ce4d850b9d72f7ef1ec/image(9).png)

* 2 Churn rate by Internation and voice mail plan

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/6a7e2b1e4c86b42897798ce4d850b9d72f7ef1ec/image(7).png)

* 3 Class distribution of churn

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/6a7e2b1e4c86b42897798ce4d850b9d72f7ef1ec/image(2).png)

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/6a7e2b1e4c86b42897798ce4d850b9d72f7ef1ec/image(3).png)

* 4 Features correlated with churn

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/6a7e2b1e4c86b42897798ce4d850b9d72f7ef1ec/image(8).png)

* 5 Correlatio matrix heatmap

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/6a7e2b1e4c86b42897798ce4d850b9d72f7ef1ec/image(13).png)


# Feature engineering

Added new features for better modelling
 - total minutes
 - total calls
 - avg minutes per call 
 - day to eve minutes ratio 
 - night to intl minutes ratio 
 - voicemail usage
 - service call ratio 
 - log total intl minutes 
 - log customer service call



# Feature importance

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/833f663d58488935771e428fcd318d25164e318c/image(15).png)



# Modeling

The XGBoost algorithm was used to predict churn. Key steps included:

- Splitting the data into training and testing sets.

- Handling class imbalance using scale_pos_weight.

- Tuning hyperparameters using GridSearchCV.


# Model Performance

The model achieved strong performance metrics:

- Accuracy: 95%
- Recall (Churn): 78%
- ROC AUC Score: 0.9096

Classification Report 

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/82ae6bc2cf79b0e51515a5ca874b08bfcd2fce8c/image(14).png)


# ROC curve

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/82ae6bc2cf79b0e51515a5ca874b08bfcd2fce8c/Screenshot%202025-02-20%20184242.png)


# Confusion matrix

![image alt](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/82ae6bc2cf79b0e51515a5ca874b08bfcd2fce8c/Screenshot%202025-02-20%20184216.png)

Access presentation slides [Here](https://github.com/Vincent-lab-create/SyriaTel-Customer-churn-Prediction/blob/d2c25d0d11623d52c6375590d0f7b6c606844755/Syria%20Tel%20churn%20prediction%20-%20Google%20Slides.pdf)

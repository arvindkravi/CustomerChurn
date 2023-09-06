# CustomerChurn
# Aim of the project is to predict the customer churn for ABC Bank
# Model - Chose logistic instead of linear regression because the dependent variable is categorical.
# 1. Preprocessed the data - checked for null, converted categorical variables to numerical to run regression. 
#2. Standardized the data - the columns tenure, balance and estimated salary will be in 1000s (different unit). To make it unit free, we standardized the data using StandardScalar
3. Next, we split the data into 80-20 train and test. Then we trained a model using logistic regression.
4. To calculate the accuracy of our model, we used a confusion matrix and accuracy score. The accuracy was 81.3%
5. We also trained another model using the K nearest neighbors (KNN) method. To find the best value for k, we classified and calculated the accuracy score for k=1 to 20. The accuracy was the highest at k=10, but since we believed it may be overfitting the model, we decided that k=5 would be the best fit for the purpose of our study. The accuracy score for this model was 80.05%
6. Using the two models above, we used predict_proba() to predict the probability of customer churn for an individual customer given some metrics such as age, salary, tenure etc.,. This would be helpful to banks to identify the customers that have a high probability of leaving the bank in the future and target them with the right products and tailor marketing strategies.(Real-world business application)
7. To test our model's performance, we generated a mock data set with 1000 records and used our model to predict whether or not a customer will be leaving the bank.

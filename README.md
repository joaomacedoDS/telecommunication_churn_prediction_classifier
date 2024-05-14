# telecommunication_churn_prediction_classifier
This project attempts to predict whether a customer will change telecommunications provider
This will be done by making a model which will be split for testing, after being trained.
Another dataset will be used for integrating the "Id" information of customers
Evaluation: The quality of such model will stated by its accuracy on the following metric:
ACCURACY = Nº CORRECT PREDICTIONS / Nº TEST SAMPLES
Goal: Provide a list which contains customers' ID along with the information whether they are a pontention "churn" or not

## Business Problem

What problem are we solving? 
It is inteded to predict which customers are very likely to cancel their account, in other words, to become a "churn".

What is "Churn"? 
According to dictionary, it's a rate of change that occurs in a business over a period of time as existing customers are lost and new customers are added. In business, on daily basis, when a customer is a "churn", it means one is likely to cancel account and/or not be a customer anymore.

What is the benefit from solving it? 
It is a critical prediction for many businesses because acquiring new clients often costs more than retaining existing ones. Once you can identify those customers that are at risk of cancelling, you should know exactly what marketing action to take for each individual customer to maximise the chances that the customer will remain.

## Important files
data source[https://www.kaggle.com/c/customer-churn-prediction-2020/overview]
main data[https://github.com/joaomacedoDS/telecommunication_churn_prediction_classifier/blob/master/train.csv]
Project Development step by step[https://github.com/joaomacedoDS/telecommunication_churn_prediction_classifier/blob/master/telecommunication_churn_classifier.ipynb]

## Results

It has been able to reach an accuracy of approximately 96% (95,9% specifically) after processing the dataset.

As deploy, this model can be used for applying in new cases, as the example that follows with the "test" dataset

With EDA and feature selection, it has been found out that 4 main reasons impact on whether a customer is a potential churn:

- Charges: By speanding 40 dollars or more per month, a customer may consider cancelling
- International plan signup: Customers with international plan are 4 times more likely to cancel than a regular one
- Number of times has called Customer Service: By calling 4 times, a customer gets unsatisfied, and likely to cancel. The more times one has to call, the more likely is to become a churn
- Minutes on calls: The more a customer spends on the phone, the more one will be charged for that service, which can lead to be more likely to cancel


Besides predicting churns, here are some potential actions to be taken in order to reduce customer loss after what it has been found out:

- For customers who spend more than 40 dollars, give special offers, so their plans get less pricey
- Clients with international plan might consider canceling, so special packs or prices can reduce this number
- Making sure a customer does not have to call more than once the customer service to solve his or her issue

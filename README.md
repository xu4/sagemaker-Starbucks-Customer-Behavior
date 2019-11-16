# StarbucksCapstoneChallenge

## Project Overview
This project is a real-life marketing strategy study based on simulated data set that mimics customer behavior on the Starbucks rewards mobile app.

By analyzing transaction, demographic and offer data, we hope that we can better target offers towards customers with higher probability to use the offers. At the same time, customers receive personalized and relevant offers on the mobile app and get better user experience. By doing these, Starbucks could potentially maximize revenue and save on marketing and promotional costs.

## Problem Statement / Metrics 
The problems I am aiming to solve in this project are:

    1. Discover the main drivers of offer effectiveness
    Explore if we can predict whether a customer will respond to an offer.
    I plan to accomplish the tasks by following the steps here:

    2. Clean and preprocess the data: combine the offer portfolio, customer profile, and transaction data, generate label whether the customer responded to the offer or not.

    3. Build classification models to predict whether a customer will respond to an offer or not. I use a DecisionTreeClassifer performance as a baseline, comparing to random forest and gradient boosting models. Both accuracy and F1-score are used as performance metrics.
    
    4. Refine the models by tuning parameters of the models.
    Find the feature importance to identify the drivers of offer effectiveness  

## Conclusion

In this project, through data exploration and model construction, I was able to solve the two problems stated at the beginning of the notebook.

    1. Discover the main drivers of offer effectiveness:
    I found that the tenure of a member is the biggest predictor of the effectiveness of an offer. Income is a big one too. I am surprised that social channel is on the top 5 even though Web and Email channels response rate are much higher than social.

    2. Explore if we can predict whether a customer will respond to an offer:
    I constructed one model to predict whether a customer will respond to an offer. I created a response_rate feature which greatly improves the classifier performance. But the response_rate feature may not be available for new customers who has only demographical information and does not have much offer related transaction data.


## Python Libraries Used
-[Python Data Analysis Library](https://pandas.pydata.org/)  
-[Numpy](http://www.numpy.org/)  
-[Matplotlib](https://matplotlib.org/)  
-[os — Miscellaneous operating system interfaces](https://docs.python.org/3/library/os.html)  
-[scikit-learn: Machine Learning in Python](https://scikit-learn.org/stable/)  
-[Joblib: running Python functions as pipeline jobs](https://joblib.readthedocs.io/en/latest/)  
 
# Bank Churn Prediction Analysis

## Project Overview
Can we reduce customer churn by predicting which customers are at risk of churning, and predicting what their needs are in order to reduce this risk?

This project seeks to answer this question by conducting predictive analysis on customer bank churn data, obtained from Kaggle. Through the development of robust predictive models, 
the objective is to pinpoint customers most susceptible to churning and devise effective strategies to mitigate this risk, thereby enhancing customer retention and reducing overall company cost.

After importing and cleaning the data, we can gain a better understanding of our data through exploratory data analysis, and then begin creating and building our models for the predictive analysis.


## Data Preprocessing
In this section, the data will be cleaned in the following steps:

* Delete unnecessary columns: RowNumber (redundant), CustomerID (privacy), Surname (privacy).
* Change gender to binary (1 for male, 0 for female).
* Change Geography and Card Type to dummy variables.
* Rename columns.
* Check for missing values.

## Exploratory Data Analysis (EDA)
After engaging in exploratory data analysis, here is some of the information gained:
Summary of the statistics
* Mean age: 39
* Mean tenure: 5, ranging from 0-10 years
* Mean balance is 76000 but ranging from 0-250,000
* 70% have credit cards
* 50% are still active members
* 20% have complained, and 20% have exited
* Mean satisfaction score of 3/5
* 50% come from France, and split 50/50 with Germany and Spain

## Modeling
Now that we have explored our data and gained a better understanding, we can begin the modeling process. As this is a binary classification problem, logistic regression is a suitable modeling algorithm for this problem.

## Conclusion
Through meticulous data preprocessing and data exploration, we optimized the model's performance to an impressive accuracy of 99.87%. Subsequent exploratory data analysis uncovered key insights into factors influencing customer churn, such as their location. We found that the customers based in Germany have a nearly 50% chance of churning, as compared to France’s and Spain’s 20% chance of churning. This finding underscores the significance of regional dynamics and the need for specified retention strategies to address the underlying drivers of churn effectively. We also found that the age group of 45-60 are more likely to churn, and we speculated this may be due to upcoming retirement financial plans not aligning with the bank’s current options, and we propose investigating the complaints of these customers to prepare a financial plan more suited to their needs. Additionally, it was shown that optimally, customers should have about 1-2 products, and having 3 or more leads to a higher likelihood of churning. Overall, the goal of this project was successful in accurately predicting customer churn, which will henceforth enhance customer retention efforts, fortifying customer relationships, and ultimately driving sustained business growth in an increasingly competitive landscape.

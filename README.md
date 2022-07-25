# Prediction-of-Personal-Loan-Purchase-Customer-Segmentation-Analysis

:pushpin:  ## PROJECT GOALS

To analyze the effectiveness of existing marketing strategies 

To find the Machine Learning models that help in identifying potential customers 

To help financial institution in maximizing the sales performance which helps a strong growth in market share

## :question: RESEARCH QUESTIONS
1. What are the most important features influencing the loan purchasing decision? And why?
2. How are the features correlated to each other?
3. What are the key characteristics of each cluster among the sample population? 
4. Which machine learning approach could be best to predict personal loan acceptance rate using the financial sector data?
5. What are the solutions for the next marketing campaign? 


## DATA SOURCE
Kaggle: https://www.kaggle.com/teertha/personal-loan-modeling

The dataset has 5000 Records and 14 Features.
ID					
Education
Age
Experience
Mortgage
Income
ZIP Code
Family
CCAvg
Personal Loan
Securities Account
CD Account
Online
CreditCard

## DESCRIPTIVE ANALYSIS

#### CORRELATION AMONG FEATURES

<img width="551" alt="image" src="https://user-images.githubusercontent.com/64395120/180674350-58adb09e-cd37-4c5d-8abd-cbbeba5b0e34.png">

Age and Experience: a strong positive correlation (r = 0.99)
Income and CCAvg: a moderate positive correlation (r = 0.65)
Age and Mortgage: a weak negative correlation (r = -0.01)
Income and Mortgage: a weak positive correlation  (r = 0.21)

#### K-MEANS CLUSTERING

<img width="378" alt="image" src="https://user-images.githubusercontent.com/64395120/180674478-def18e0a-1df1-4fae-8b66-26d27e55dcd9.png">
Cluster 1: Younger population, lower income
Cluster 2: Older population, mostly lower income
Cluster 3: Mostly middle age population, higher income	

## PREDICTIVE ANALYSIS

Candidate 1: k-NN
<img width="204" alt="image" src="https://user-images.githubusercontent.com/64395120/180674577-307b8b7f-9142-4129-8178-a26ce91cabeb.png">
<img width="132" alt="image" src="https://user-images.githubusercontent.com/64395120/180674587-699cb671-8c36-496f-8af7-8b80e9fbd2de.png">

Candidate 2: Logistic Regression
<img width="218" alt="image" src="https://user-images.githubusercontent.com/64395120/180674617-c09a39f7-8166-4b68-b060-e04998161203.png">

Automatic Parameter Tuning was used when creating most of the models

Candidate 3: Decision Tree
<img width="236" alt="image" src="https://user-images.githubusercontent.com/64395120/180674664-bd5e04f1-1344-4809-9c61-b455b8cfd682.png">
<img width="160" alt="image" src="https://user-images.githubusercontent.com/64395120/180674676-0c02fe06-5cff-4d1d-a28c-6d910a0daa04.png">

Candidate 4: Random Forest 
<img width="258" alt="image" src="https://user-images.githubusercontent.com/64395120/180674702-6110cdd7-ffd3-41cc-a39e-8c6595b36013.png">
<img width="250" alt="image" src="https://user-images.githubusercontent.com/64395120/180674710-93098ac6-8bfe-40e2-b6b4-96fa8a5ae9f1.png">

Model for deployment is Random Forest

Automatic parameter tuning
<img width="219" alt="image" src="https://user-images.githubusercontent.com/64395120/180674739-623d6fb1-e3d4-49cf-a347-47b8d1f3ef9c.png">


## CONCLUSION

Our decision tree model indicates these features are the most important deciding factors influencing the loan purchasing decision are Age, Income, CCAvg, Education

Target the untapped customer base for personal loan market
      CLUSTER 3	
      Higher Income
      CCAVG: Higher spending 
      Mortgage: Yes
      Securities Account: Yes
      CD Account: Yes
      Online: Active online user
      Credit Card with another bank
      Reason: features suggest lower default risk
 
      CLUSTER 1  		
      Younger generation
      Population density
      CCAVG: less spending 
      Mortgage: lower amount
      Reason: large population size with potential of goodwill

Decision Tree and Random Forest appeared to be the best models with highest performance in our scenario


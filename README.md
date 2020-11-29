# Starbucks-Capstone-Project
Starbucks, as a marketing strategy, provides discounts or free services on its offerings to users. 
An offer can be merely an Information for a drink or an actual offer such as a Discount or Buy One Get One.
These offerings help in increasing sales and creating customer awareness of new products. 
Starbucks has a diverse user base. Hence not all offers are rolled out to each customer. 
Starbucks gives different offers to different customers based on their demographics and user profile. 
In a simple words Starbucks’ offering are personalised. Business lean towards propensity model to reduce the expenditure in advertising, as model give them more specific target customer.

In this project our main task is to combine user data, offering details and transaction data to determine is their any affinity between user attributes and a offer type.

## Table Of Contents   
* [Summary](#summary)  
* [File Description](#description)  
* [Libraries](#library)
* [Running the Application](#execution)
* [Licensing, Authors, Acknowledgements](#compliance)


<a name="summary"></a>
## Summary 
The project was completed in the following phases:
* Dataset Exploration:- In this process, the data provided was loaded to see how it looks like.
* Dataset Claening/Transformation:- In this phase changes were made to dataset to make it more meaningful and logical.
* Combining the three DataSet:- Once initial data explorationa and cleaning was done all dataset were combined.
* Target varible generation.
* EDA on the combined dataset:- This looked into dataset distribution and its relation with the target variable.
* Modelling and Performance Evaluation: In this step, various machine learning model(Decision Tree, KNN, Logistic Regression and Random Forest) were tested on the given dataset and their respective performances was recorded. 


<a name="description"></a>
## File Descriptions
#### Data Dictionary
##### profile.json
Rewards program users (17000 users x 5 fields)

gender: (categorical) M, F, O, or null   
age: (numeric) missing value encoded as 118   
id: (string/hash)   
became_member_on: (date) format YYYYMMDD   
income: (numeric)      

##### portfolio.json
Offers sent during 30-day test period (10 offers x 6 fields)

reward: (numeric) money awarded for the amount spent   
channels: (list) web, email, mobile, social   
difficulty: (numeric) money required to be spent to receive reward   
duration: (numeric) time for offer to be open, in days   
offer_type: (string) bogo, discount, informational   
id: (string/hash)     
 
##### transcript.json
Event log (306648 events x 4 fields)

person: (string/hash)   
event: (string) offer received, offer viewed, transaction, offer completed   
value: (dictionary) different values depending on event type   
offer id: (string/hash) not associated with any "transaction"   
amount: (numeric) money spent in "transaction"   
reward: (numeric) money gained from "offer completed"   
time: (numeric) hours after start of test   

<a name="library"/></a>
## Libraries

This project is developed in Python 3.6.
Below library were used.

jupyter
numpy
pandas
seaborn
scikit-learn 

<a name="execution"/></a>
## Running the Application
Keep the three files (portfolio, profile, transcript) in Data folder.
Open IPython notebook file in the project directory and execute each cell.

<a name="compliance"/></a>
## Licensing, Authors, Acknowledgements
Dataset provided is by Udacity on behalf of Starbucks.




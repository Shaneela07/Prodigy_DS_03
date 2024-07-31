# Prodigy_DS_03
# Term Deposit Prediction on Bank Marketing campaigns (phone calls)
Build a Decision Tree classifier to predict if the client will subscribe to a Term Deposit based on their demographic and behavioural data.

# Dataset
This dataset is a Bank Marketing dataset from the UCI Machine Learning Repository (https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) The data is related to a Portuguese banking institution's direct marketing campaigns (phone calls). Often, more than one contact to the same client was required, to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

# Column Description:
age : Integer Age

job: Occupation

marital: Marital Status

education: Education Level

default: has credit in default?

balance: average yearly balance in euros

housing: has housing loan?

loan : has a personal loan?

contact : contact communication type

day_of_week : last contact day of the week

duration : last contact duration, in seconds (numeric)

campaign : number of contacts performed during this campaign and for this client

pdays : number of days that passed by after the client was last contacted from a previous campaign(numeric, -1 means client was not previously contacted)

previous : number of contacts performed before this campaign and for this client

poutcome : outcome of the previous marketing campaign

emp.var.rate: employment variation rate - quarterly indicator (numeric)

cons.price.idx: consumer price index - monthly indicator (numeric)

cons.conf.idx: consumer confidence index - monthly indicator (numeric)

euribor3m: euribor 3 month rate - daily indicator (numeric)

nr.employed: number of employees - quarterly indicator (numeric)

deposit : has the client subscribed a term deposit? (outcome)

# Conclusion and Key Insights

In this project, we embarked on a journey to build a predictive model for term deposit subscriptions in a banking context to help a Portuguese banking institution tailor its marketing efforts effectively. Let's recap the key takeaways and insights from this endeavour:

# Data Pre-processing:

The initial data inspection revealed a well-structured dataset with no missing values. While we encountered some duplicate entries, they were not considered errors but rather different campaigns targeting the same clients.

# Exploratory Data Analysis (EDA):

The age distribution of clients highlighted that the majority fell in the 30-40 age range, coinciding with the highest subscription rate for term deposits.
Occupation-wise, clients in administrative, blue-collar and technician roles formed the majority and were more likely to subscribe to term deposits.
Marital status leaned heavily toward the "married" category.
Clients with university degrees or high-level education were more prominent and had a higher subscription rate.
Credit defaults were rare, with the vast majority of clients having no credit defaults.
Clients with housing loans were likelier to subscribe to term deposits, while those with personal loans were less likely.

# Model Building and Evaluation:

We implemented a Decision Tree classifier to predict term deposit subscriptions. 
The model exhibited strong performance, achieving an accuracy rate of approximately 80.29% on both training and testing data.
Cross-validation confirmed the robustness of our model, with an accuracy score of around 77.43%.

# Insights:
The duration of calls was a significant predictor of term deposit subscriptions. Clients tended to subscribe after longer conversations, suggesting the importance of engaging clients effectively during calls.
Previous attempts at contact also played a role, indicating that repeated contact can be fruitful in convincing clients to subscribe.
Multicollinearity among some input features was observed, potentially affecting model performance.

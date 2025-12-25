## Credit Card Customer_Segmentation
This dataset contains a wealth of customer information collected from within a consumer credit card portfolio, with the aim of helping analysts predict customer attrition. It includes comprehensive demographic details such as age, gender, marital status and income category, as well as insight into each customer’s relationship with the credit card provider such as the card type, number of months on book and inactive periods. Additionally it holds key data about customers’ spending behavior drawing closer to their churn decision such as total revolving balance, credit limit, average open to buy rate and analyzable metrics like total amount of change from quarter 4 to quarter 1, average utilization ratio and Naive Bayes classifier attrition flag (Card category is combined with contacts count in 12months period alongside dependent count plus education level & months inactive). Faced with this set of useful predicted data points across multiple variables capture up-to-date information that can determine long term account stability or an impending departure therefore offering us an equipped understanding when seeking to manage a portfolio or serve individual customers

## About this file
This dataset provides customer information to predict customer attrition for a consumer credit card portfolio

CLIENTNUM: Unique identifier for each customer. (Integer)
Attrition_Flag: Flag indicating whether or not the customer has churned out. (Boolean)
Customer_Age: Age of customer. (Integer)
Gender: Gender of customer. (String)
Dependent_count: Number of dependents that customer has. (Integer)
Education_Level: Education level of customer. (String)
Marital_Status: Marital status of customer. (String)
Income_Category: Income category of customer. (String)
Card_Category: Type of card held by customer. (String)
Months_on_book: How long customer has been on the books. (Integer)
Total_Relationship_Count: Total number of relationships customer has with the credit card provider. (Integer)
Months_Inactive_12_mon: Number of months customer has been inactive in the last twelve months. (Integer)
Contacts_Count_12_mon: Number of contacts customer has had in the last twelve months. (Integer)
Credit_Limit: Credit limit of customer. (Integer)
Total_Revolving_Bal: Total revolving balance of customer. (Integer)
Avg_Open_To_Buy: Average open to buy ratio of customer. (Integer)
Total_Amt_Chng_Q4_Q1: Total amount changed from quarter 4 to quarter 1. (Integer)
Total_Trans_Amt: Total transaction amount. (Integer)
Total_Trans_Ct: Total transaction count. (Integer)
Total_Ct_Chng_Q4_Q1: Total count changed from quarter 4 to quarter 1. (Integer)
Avg_Utilization_Ratio: Average utilization ratio of customer. (Integer)
Naive_Bayes_Classifier_Attrition_Flag_Card_Category_Contacts_Count_12_mon_Dependent_count_Education_Level_Months_Inactive_12_mon_1: Naive Bayes classifier for predicting whether or not someone will churn based on characteristics such
Tools Used
Numpy
Pandas
Matplotlib
Seaborn
Scikit-learn
Plotly
What we will do:
Reading the data
Data Cleaning
Dealing with duplicates
Dealing with irrelevant columns
Dealing with outliers
Exploratory Data Analysis
Data Preparation
Data Preparation
Label Encoding
Scaling
Dimentionality Reduction
Model Building with Kmeans Algorithm
Customer Profiling
KMeans Clustering and how it works?
K-Means Clustering is an Unsupervised Machine Learning algorithm, which groups the unlabeled dataset into different clusters. The algorithm assigns data points to one of the K clusters depending on their distance from the center of the clusters. It starts by randomly assigning the clusters centroid in the space. Then each data point assign to one of the cluster based on its distance from centroid of the cluster. After assigning each point to one of the cluster, new cluster centroids are assigned. This process runs iteratively until it finds good cluster. In the analysis we assume that number of cluster is given in advanced and we have to put points in one of the group.

# 💳 Credit Card Customer Segmentation Using Clustering Analysis
## 📌 Project Overview
This project focuses on customer segmentation for a credit card business using **unsupervised machine learning techniques.** By analyzing demographic, behavioral, and transactional attributes, the goal is to identify distinct customer groups that differ in spending behavior, credit usage, engagement level, and attrition risk.

Through **exploratory data analysis (EDA)**, **data preprocessing**, **dimensionality reduction**, and **KMeans clustering**, the project uncovers meaningful customer segments that can help financial institutions design targeted marketing strategies, retention plans, and personalized credit offerings.
___
## 📊 Dataset Description
Each row represents a unique credit card customer along with their demographic profile, account information, and transaction behavior.

Key Features Include:

**CLIENTNUM:** Unique identifier for each customer. (Integer)

**Attrition_Flag:** Flag indicating whether or not the customer has churned out. (Boolean)

**Customer_Age:** Age of customer. (Integer)

**Gender:** Gender of customer. (String)

**Dependent_count:** Number of dependents that customer has. (Integer)

**Education_Level:** Education level of customer. (String)

**Marital_Status:** Marital status of customer. (String)

**Income_Category:** Income category of customer. (String)

**Card_Category:** Type of card held by customer. (String)

**Months_on_book:** How long customer has been on the books. (Integer)

**Total_Relationship_Count:** Total number of relationships customer has with the credit card provider. (Integer)

**Months_Inactive_12_mon:** Number of months customer has been inactive in the last twelve months. (Integer)

**Contacts_Count_12_mon:** Number of contacts customer has had in the last twelve months. (Integer)

**Credit_Limit:** Credit limit of customer. (Integer)

**Total_Revolving_Bal:** Total revolving balance of customer. (Integer)

**Avg_Open_To_Buy:** Average open to buy ratio of customer. (Integer)

**Total_Amt_Chng_Q4_Q1:** Total amount changed from quarter 4 to quarter 1. (Integer)

**Total_Trans_Amt:** Total transaction amount. (Integer)

**Total_Trans_Ct:** Total transaction count. (Integer)

**Total_Ct_Chng_Q4_Q1:** Total count changed from quarter 4 to quarter 1. (Integer)

**Avg_Utilization_Ratio:** Average utilization ratio of customer. (Integer)

**Naive_Bayes_Classifier_Attrition_Flag_Card_Category_Contacts_Count_12_mon_Dependent_count_Education_Level_Months_Inactive_12_mon_1:** Naive Bayes classifier for predicting whether or not someone will churn based on characteristics such.
___

### Dataset Cleaning Highlights:

- Dropped columns related to pre-computed Naive Bayes scores

- Removed rows containing Unknown values in: Education_Level, Marital_Status, Income_Category
  
- Removed outliers using the IQR method
___
## 🛠️ Skills & Tools Used
- **Programming & Libraries**

  - **Python:** Pandas, NumPy

  - **Data Visualization:** Matplotlib, Seaborn, Plotly, heatmaps

  - **Machine Learning:** Scikit-learn

- **Data Processing & Feature Handling**

  - Label Encoding for categorical variables

  - Standard Scaling for numerical features

  - Outlier detection using IQR method

- **Dimensionality Reduction**

  - Principal Component Analysis (PCA)

  - Reduced high-dimensional data to 3 components for visualization and clustering

- **Clustering & Evaluation**

  - KMeans Clustering

  - Silhouette Score to determine optimal number of clusters
___
## 🔎 Exploratory Data Analysis (EDA) – Key Insights
- **Customer Attrition**

  - Around ~16% customers have attrited, while ~84% remain active.

- **Demographics**

  - Average customer age is ~46 years, ranging from 26 to 73.

  - Gender distribution is fairly balanced.

  - Most customers are graduates and married.

- **Income & Card Usage**

  - Customers earning less than $40K annually form the largest group.

  - Blue cards are the most widely used, while Platinum cards are rare.

- **Activity & Engagement**

  - Average tenure with the bank is 36 months.

  - Majority of customers were inactive for 2–3 months in the last year.

  - Most customers contacted the bank 2–3 times annually.

- **Correlation Insights**

  - Strong positive correlation between total transaction amount & transaction count.

  - Credit limit shows negative correlation with utilization ratio and positive relationship with “open to buy”.

  - Several monetary features show positive skewness, motivating outlier handling.
___
## 🤖 Modeling Approach
- **Data Preparation**

  - Encoded categorical variables using Label Encoding

  - Scaled all features using StandardScaler

- **Dimensionality Reduction**

  - Applied PCA (3 components) to enable visualization and improve clustering efficiency

- **Optimal Cluster Selection**

  - Evaluated clusters from k = 2 to 10 using Silhouette Score

  - Optimal number of clusters: k = 3

  - Best Silhouette Score ≈ 0.33

- **KMeans Clustering**

  - Final model built using KMeans with 3 clusters

  - Clusters visualized in 3D PCA space
___
## 📌 Customer Segments & Profiles
### 🔴 Cluster 0 – High-Value Loyal Customers

- High credit limit, medium transaction amount

- Median age ≈ 46 years

- Wide transaction frequency (low to very high)

- Very low attrition rate

- Moderate inactivity, regular customer engagement

**Business Insight:**
This segment represents financially stable and loyal customers.
They should be prioritized for:

- Credit limit upgrades

- Premium card offers

- Exclusive loyalty rewards

### 🟢 Cluster 1 – Active Mass Segment

- Low credit limit, medium transaction amount

- Large customer base

- High engagement with customer support

- Low attrition but higher inactivity periods

**Business Insight:**
This is a growth-oriented segment.
Recommended actions:

- Gradual credit limit enhancements

- Upsell opportunities

- Personalized engagement campaigns

### 🔵 Cluster 2 – High Churn Risk Customers

- Low credit limit & low transaction amount

- Median age ≈ 50 years

- Almost equal proportion of attrited and existing customers

- Lower transaction frequency

**Business Insight:**
This segment is at high risk of churn.
Retention strategies include:

- Targeted offers and incentives

- Re-engagement campaigns

- Lower-fee card alternatives
___
## 🧠 Business Value

- Enables customer-centric marketing strategies

- Helps banks proactively reduce customer churn

- Supports risk-based segmentation and smarter credit decisions

- Improves allocation of retention and loyalty budgets
___
## 📌 Conclusion

- This project demonstrates how unsupervised learning techniques, combined with thorough EDA and dimensionality reduction, can uncover actionable customer segments in the credit card domain.

- By translating raw transaction and demographic data into clear customer personas, the analysis bridges the gap between data science and real-world business strategy—making it valuable for both academic learning and financial industry applications.

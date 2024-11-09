# Customer Personality Clustering to Boost Marketing Campaigns

## Objective:
The project aims to improve the marketing conversion rate (CR) by clustering customers based on their behavior and characteristics. By understanding different customer segments, we can tailor marketing strategies to boost campaign effectiveness.

## Project Overview:
Using data from a marketing campaign, this project applies machine learning techniques to segment customers into meaningful groups. The goal is to identify key characteristics that influence spending habits and conversion rates, which can inform targeted marketing strategies.

## Dataset Description:
The dataset contains information about customer demographics, spending behavior, and marketing campaign responses. Key fields include:

-Demographic Information: Year_Birth, Education, Marital_Status, Income, Kidhome, Teenhome

-Customer Engagement: Dt_Customer, Recency, NumWebVisitsMonth

-Spending: MntCoke, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts, MntGoldProds

-Purchases: NumDealsPurchases, NumWebPurchases, NumCatalogPurchases, NumStorePurchases

-Campaign Responses: AcceptedCmp1, AcceptedCmp2, AcceptedCmp3, AcceptedCmp4, AcceptedCmp5, Response


## Feature Engineering

-CR: Conversion rate, calculated as Response / NumWebVisitsMonth

-Age: Customer age, derived from Year_Birth

-Children: Total number of children, calculated as Kidhome + Teenhome

-Total_Spend: Sum of all product spending

-Purchases: Total number of purchases across different channels

-Member_Period: Number of years since becoming a member, calculated from Dt_Customer


## Methodology

### Data Preprocessing

Handled missing values and outliers.
Standardized the data using Min-Max Scaler.
Encoded categorical features (Education and Marital_Status) using One Hot Encoding.

### Exploratory Data Analysis (EDA)

Analyzed correlations and relationships between features.
Identified features like Total_Spend, AcceptedCmp5, and Children as important for clustering.

### Clustering

Used K-Means Clustering to segment customers.
Evaluated different numbers of clusters using the silhouette score, selecting the optimal number based on a balance between score and interpretability.
Results

## Clustering identified five distinct customer segments:

Cluster 0: Moderate spenders with children and low CR.

Cluster 1: High spenders with high CR and few children.

Cluster 2: Low to moderate spenders with many children and low CR.

Cluster 3: High spenders with children but low CR.

Cluster 4: High spenders without children and moderate CR.

## Conclusion

The clustering analysis provides insights into customer behavior, helping to tailor marketing strategies for each segment. High-value segments can be targeted with premium offers, while family-oriented customers might respond better to value-driven campaigns.

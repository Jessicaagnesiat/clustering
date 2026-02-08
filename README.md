# Airline Customer Segmentation using K-Means and Agglomerative Clustering

## Overview
Understanding customer behavior is critical for airline companies to improve loyalty, retention, and revenue.  
This project segments airline customers based on flight activity, spending behavior, and loyalty metrics using unsupervised learning techniques.

## Problem Statement
Airline customer data contains complex behavioral patterns that cannot be effectively analyzed using raw metrics alone, making it difficult to distinguish high-value loyal customers from low-engagement travelers.

## Objectives
- Segment airline customers based on behavioral and loyalty characteristics  
- Identify high-value and low-engagement customer groups  
- Compare clustering methods and select the most reliable model  
- Generate actionable business insights for marketing and retention strategies  

## Dataset
- **Records:** ~63,000 customers  
- **Features:** Flight activity, loyalty tier, spending, distance traveled, points usage, tenure, and recency  
- **Type:** Customer loyalty and flight behavior data  

## Methodology
1. **Data Cleaning & Preprocessing**
   - Removed irrelevant and high-cardinality categorical features
   - Handled missing values and duplicates
   - Converted date features to datetime
2. **Feature Engineering**
   - Tenure, recency, flight frequency
   - Average flight distance
   - Unused loyalty point ratio
3. **Feature Scaling**
   - Applied StandardScaler to normalize numerical features
4. **Clustering Models**
   - Agglomerative Clustering (sampling due to memory constraints)
   - K-Means Clustering (full dataset)
5. **Model Evaluation**
   - Silhouette Score
   - Calinski-Harabasz Index
6. **Visualization**
   - Dendrogram
   - PCA-based 2D cluster visualization

## Results
Two distinct customer segments were identified:
- **High Value Loyal Flyers**
  - Frequent and long-distance travelers
  - High spending and active loyalty point usage
  - Long membership tenure
- **Low Engagement Casual Travelers**
  - Infrequent and short-distance travelers
  - Low spending and minimal point usage
  - Higher inactivity and churn risk

K-Means clustering was selected as the final model due to better scalability and use of the full dataset.

## Business Impact
- Enables targeted loyalty programs for high-value customers
- Supports re-engagement campaigns for low-activity customers
- Improves customer lifetime value and retention
- Helps optimize promotional and loyalty reward strategies

## Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib

## Conclusion
Customer segmentation using K-Means clustering effectively distinguishes airline customers into meaningful behavioral groups, providing actionable insights for loyalty management and marketing optimization.

## Author
Jessica Agnesia Tataung

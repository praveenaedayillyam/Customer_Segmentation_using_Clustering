# Customer_Segmentation_using_Clustering

🛍️ Customer Segmentation using K-Means Clustering
📌 Project Overview

Customer segmentation is a crucial marketing strategy that helps businesses understand customer behavior and target them effectively.
This project applies K-Means Clustering to segment customers based on income, spending behavior, and demographic features.

Using feature engineering, data preprocessing, PCA for dimensionality reduction, and the Elbow Method, customers are grouped into meaningful clusters that reveal actionable business insights.

🎯 Objectives

Perform customer segmentation using unsupervised learning

Identify distinct customer groups based on spending patterns and income

Reduce dimensionality using Principal Component Analysis (PCA)

Determine the optimal number of clusters using the Elbow Method

Visualize and interpret customer segments for targeted marketing

📂 Dataset

Source: marketing_campaign.csv

Records: 2240 customers

Features: Demographics, spending behavior, purchase channels, campaign responses

🧹 Data Cleaning & Feature Engineering

Key preprocessing steps include:

Removed missing values in Income

Converted customer enrollment date into Customer_For (days registered)

Created new features:

Age

Spent (total spending across product categories)

Children

Family_Size

Is_Parent

Living_With

Consolidated education levels into:

Undergraduate

Graduate

Postgraduate

Removed redundant and non-informative columns

Capped outliers in Age and Income

🔄 Data Preprocessing

Label encoded categorical variables:

Education

Living_With

Removed campaign-related columns to avoid bias

Applied StandardScaler for feature scaling

📉 Dimensionality Reduction (PCA)

Reduced dataset to 3 principal components

Enabled effective 3D visualization

Preserved maximum variance for clustering

🧠 Clustering Approach
🔹 Elbow Method

Used Yellowbrick’s KElbowVisualizer

Optimal number of clusters identified: 4

🔹 K-Means Clustering

Applied K-Means with n_clusters = 4

Cluster labels added back to the original dataset

📊 Visualizations

3D PCA scatter plot

Cluster distribution count plot

Income vs Spending scatter plot

These visualizations clearly show separable customer segments.

📌 Customer Segments Identified

Based on Income vs Spending patterns:

Low Income – Low Spending

Medium Income – Medium Spending

High Income – High Spending

Very High Income – Moderate to High Spending

💡 Business Insights

Enables targeted marketing strategies

Helps identify premium customers

Supports better customer retention and personalization

Assists businesses in allocating marketing resources effectively

🛠️ Technologies & Libraries Used

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

Yellowbrick

# Customer-Segmentation-using-K-Means-Clustering
## 📌 Overview
This project performs customer segmentation using unsupervised learning on large-scale retail transaction data. The objective is to group customers based on purchasing behavior to support targeted marketing, retention strategies, and business decision-making.

## 📂 Dataset
* Source: UCI Machine Learning Repository
* Dataset: Online Retail
* Records: 500,000+ transaction records
* Customers: ~4,000 unique customers
## Key Columns
* CustomerID
* InvoiceNo
* InvoiceDate
* Quantity
* UnitPrice
* Country
The raw transactional data was cleaned and aggregated to customer-level features before clustering.

## ⚙️ Tech Stack
* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

## 🔄 Project Workflow
1. Problem Framing Segmentation of customers using unsupervised learning (no labels available).
2. Data Cleaning
    * Removed missing CustomerID
    * Removed cancelled/returned transactions
    * Filtered invalid quantities and prices
3. Feature Engineering (RFM Analysis)
    * Recency: Days since last purchase
    * Frequency: Number of transactions
    * Monetary: Total spending
4. Exploratory Data Analysis (EDA)
    * Analyzed feature distributions and skewness
    * Identified need for feature scaling
5. Clustering
    * Applied K-Means clustering
    * Optimized number of clusters using Elbow Method and Silhouette Score
6. Dimensionality Reduction
    * Used PCA for 2D visualization of customer segments

## 📊 Results
* Successfully identified distinct customer segments
* Clear separation between:
    * High-value loyal customers
    * Frequent low-spend customers
    * At-risk or churn-prone customers
    * Occasional buyers

## 💡 Business Impact
* Enables targeted marketing campaigns
* Helps prioritize high-value customers
* Identifies churn-risk customers for retention strategies

## ⚠️ Limitations
* Clusters are sensitive to outliers
* No ground-truth labels for validation
* Segmentation quality depends on feature engineering

## 🚀 Future Improvements
* Try alternative clustering methods (DBSCAN, Hierarchical)
* Add temporal features
* Evaluate cluster stability over time


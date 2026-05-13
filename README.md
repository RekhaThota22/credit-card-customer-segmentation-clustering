# Credit Card Customer Segmentation using Unsupervised Learning

## Project Overview
This project performs customer segmentation on credit card users using unsupervised machine learning techniques to identify distinct customer behavior groups.

The objective was to discover natural customer segments based on financial activity, spending behavior, and credit usage patterns to support business decision-making.

---

## Dataset Features
Behavioral financial attributes included:

- BALANCE
- BALANCE_FREQUENCY
- PURCHASES
- ONEOFF_PURCHASES
- INSTALLMENTS_PURCHASES
- CASH_ADVANCE
- PURCHASES_FREQUENCY
- ONEOFF_PURCHASES_FREQUENCY
- PURCHASES_INSTALLMENTS_FREQUENCY
- CASH_ADVANCE_FREQUENCY
- CASH_ADVANCE_TRX
- PURCHASES_TRX
- CREDIT_LIMIT
- PAYMENTS
- MINIMUM_PAYMENTS
- PRC_FULL_PAYMENT
- TENURE

Identifier removed:
- CUST_ID

---

## Project Workflow

### Data Preprocessing
- Dataset inspection
- Null value handling using median imputation
- Duplicate check
- Identifier removal
- Column standardization
- Feature scaling using StandardScaler

---

## Clustering Techniques Used

### KMeans Clustering
Implemented:
- Elbow Method (WCSS)
- Silhouette Score validation
- Cluster assignment

### Dimensionality Reduction
- PCA (2D visualization of clusters)

### Density-Based Clustering
- DBSCAN implementation
- eps tuning experiments
- noise detection analysis

---

## Key Findings

KMeans identified meaningful customer segments such as:

- Premium High-Spending Customers
- High Credit Dependency Customers
- Regular Responsible Customers
- Low Engagement Customers
- Inactive Customers

DBSCAN was also evaluated, but due to the high-dimensional financial dataset, it produced excessive noise points and less actionable segmentation compared to KMeans.

---

## Business Applications
Customer segmentation can support:

- targeted marketing campaigns
- premium customer retention
- risk monitoring
- dormant customer reactivation
- credit behavior analysis

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Machine Learning Concepts Covered
- Unsupervised Learning
- KMeans Clustering
- Elbow Method
- Silhouette Score
- PCA
- DBSCAN
- Density-Based Clustering

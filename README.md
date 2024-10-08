# Crypto Clustering

## Overview
The Crypto Clustering project utilizes unsupervised learning techniques to analyze and cluster various cryptocurrencies based on their price change percentages over 24 hours and 7 days. The analysis aims to identify patterns in cryptocurrency behavior and optimize clustering through Principal Component Analysis (PCA).

## Data Source
The data for this project is obtained from the `crypto_market_data.csv` file, which contains various metrics of cryptocurrencies.

## Methodology
1. **Data Preparation**:
   - Load the data and generate summary statistics.
   - Normalize the data using StandardScaler.

2. **Finding the Best Value for k**:
   - Utilize the elbow method to determine the optimal number of clusters.

3. **Clustering**:
   - Implement K-Means clustering on the scaled data.
   - Visualize the clustering results using scatter plots.

4. **Principal Component Analysis (PCA)**:
   - Reduce dimensions using PCA to enhance clustering efficiency.
   - Re-evaluate the optimal number of clusters using PCA data.

5. **Comparison**:
   - Compare clustering results from the original scaled data with those from the PCA data through composite plots.

## Results
- The analysis identified the best k value for clustering:
  - Original Data: **4**
  - PCA Data: **3**
- Composite plots visually represent the differences in clustering results between the two methods.

## Conclusions
The project demonstrates the effectiveness of clustering cryptocurrencies based on their price changes. The use of PCA provided a means to simplify the dataset while retaining significant variance, leading to more efficient clustering.

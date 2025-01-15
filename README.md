# Cryptocurrency Clustering Project

## Overview

This project is a challenge for an AI Boot Camp where we apply machine learning techniques to cluster cryptocurrencies based on their price fluctuations. By using K-Means clustering and Principal Component Analysis (PCA), we analyze and visualize how cryptocurrencies are grouped based on historical price change data.

## Objectives

The primary goals of this project include:

- Applying the K-Means algorithm to cluster cryptocurrencies based on scaled price data.

- Using PCA to reduce the dimensionality of the data while retaining key information.

- Visualizing the clusters to better understand the groupings and influences of different features.

## Dataset

The data for this project is stored in a CSV file (crypto_market_data.csv) and contains the following columns:

*price_change_percentage_24h*

*price_change_percentage_7d*

*price_change_percentage_14d*

*price_change_percentage_30d*

*price_change_percentage_60d*

*price_change_percentage_200d*

*price_change_percentage_1y*

## Preprocessing Steps

- Scaling: The data was normalized using StandardScaler from scikit-learn to ensure all features are on the same scale.

- Dimensionality Reduction: PCA was applied to reduce the dataset to three principal components while retaining significant variance.

## Implementation

The project was implemented in Python, using the following key libraries:

- **pandas:** For data manipulation and analysis.

- **scikit-learn:** For K-Means clustering, PCA, and scaling.

- **matplotlib:** For creating visualizations.

## Key Steps

1. Data Preparation:

    - Load the dataset into a DataFrame.

    - Normalize the data using StandardScaler.

2. Finding the Optimal Number of Clusters:

    - Use the Elbow Method on both the original scaled data and the PCA-transformed data.

3.  Clustering Cryptocurrencies:

    - Apply the K-Means algorithm to both the original scaled data and PCA-transformed data.

    - Visualize the resulting clusters.

4. Feature Influence Analysis:

    - Examine the weights of each feature on the principal components to identify key drivers of variance.

## Results

- The optimal number of clusters (‘k’) was determined to be 4 using the Elbow Method for both original and PCA data.

- PCA reduced the dimensionality of the data to three principal components, explaining approximately X% of the variance (replace with calculated value).

- Key features influencing each principal component were identified, providing insights into the driving factors behind the clustering.

## Visualizations

- Elbow curves for determining the optimal number of clusters.

- Scatter plots showing clusters on the original scaled data and PCA-transformed data.

- PCA feature influence matrix for understanding the impact of individual features.

## Conclusion

This project successfully demonstrates the application of K-Means clustering and PCA in grouping cryptocurrencies based on their price fluctuations. By reducing dimensionality and analyzing feature influences, we gained a deeper understanding of the relationships between different cryptocurrencies.

## Future Work

- Incorporate additional features such as market capitalization and trading volume to enhance clustering.

- Experiment with other clustering algorithms (e.g., DBSCAN or Agglomerative Clustering).

- Develop interactive visualizations for better exploration of the clustering results.

## Acknowledgments

This project is part of the AI Boot Camp Challenge, designed to enhance hands-on experience in machine learning techniques. Special thanks to the boot camp instructors and peers for their guidance and collaboration.

## References

- scikit-learn documentation: https://scikit-learn.org

- Matplotlib documentation: https://matplotlib.org


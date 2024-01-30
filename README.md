# Unsupervised Machine Learning Program README

## Introduction
This Python script demonstrates the application of unsupervised machine learning techniques, specifically K-Means clustering, on cryptocurrency market data. The program utilizes libraries such as pandas, hvplot, and scikit-learn to perform data analysis, preprocessing, and clustering.

## Prerequisites
Before running the script, ensure you have the following Python libraries installed:
- pandas
- hvplot
- scikit-learn

You can install these libraries using the following command:
```bash
pip install pandas hvplot scikit-learn
```

## Usage
    . Import the required libraries and dependencies.
    . Load the cryptocurrency market data into a Pandas DataFrame from a CSV file.
    . Perform data analysis, including displaying sample data and generating summary statistics.
    . Prepare the data by normalizing it using StandardScaler from scikit-learn.
    . Find the best value for k (number of clusters) using the original data by plotting an Elbow Curve.
    . Cluster cryptocurrencies using K-Means with the original data and visualize the results.
    . Optimize clusters using Principal Component Analysis (PCA) to reduce dimensionality.
    . Find the best value for k using the PCA-transformed data and plot the Elbow Curve.
    . Cluster cryptocurrencies using K-Means with the PCA-transformed data and visualize the results.

## Results and Analysis

    * Original Data Analysis
        . The Elbow Curve analysis suggests that the optimal value for k is 4.
        . Clustering using K-Means on the original data reveals distinct clusters, visualized in a scatter plot.
    * Dimensionality Reduction with PCA
        . Principal Component Analysis (PCA) is used to reduce the dimensionality of the data to three principal components.
        . The total explained variance of the three principal components is approximately 89.50%.

    * Results with PCA Data
        .The Elbow Curve analysis using PCA-transformed data confirms that the optimal value for k is 4.
        .Clustering using K-Means on the PCA-transformed data also reveals well-defined clusters, visualized in a scatter plot.

    * Visual Comparison
        . A composite plot contrasts the Elbow curves of the original data and PCA-transformed data, emphasizing the reduction in features.
        . Scatter plots visually compare the clusters obtained from the original data and PCA-transformed data, showcasing the impact of using fewer features.

## Conclusion
    After visually analyzing the cluster analysis results, it is evident that using fewer features (after PCA) improves the quality and definition of clusters. The reduced feature set, obtained through dimensionality reduction, is effective for clustering and results in more well-defined groups compared to the original data.
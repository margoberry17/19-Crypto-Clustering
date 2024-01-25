# Crypto Clustering
Unsupervised Machine Learning &amp; Principal Component Analysis (PCA)

# Prepare the Data

    Used the StandardScaler() module from scikit-learn to normalize the data from the CSV file.

    Created a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.


# Find the Best Value for k Using the Original Scaled DataFrame

  Used the elbow method to find the best value for k. Based on the image, 4 is the best value for k.


# Cluster Cryptocurrencies with K-means Using the Original Scaled Data

  Clustered the cryptocurrencies for k=4 on the original scaled data:


# Optimize Clusters with Principal Component Analysis

  Using the original scaled DataFrame, I performed a PCA and reduced the features to three principal components.

  Retrieved the explained variance to determine how much information can be attributed to each principal component.

  Created a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.
  

# Find the Best Value for k Using the PCA Data

  Used the elbow method on the PCA data to find the best value for k.
  

# Cluster Cryptocurrencies with K-means Using the PCA Data

  Clustered the cryptocurrencies for k=4 on the PCA data.

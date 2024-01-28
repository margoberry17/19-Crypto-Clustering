# Crypto Clustering
Unsupervised Machine Learning &amp; Principal Component Analysis (PCA)

## Prepared the Data

-Used the StandardScaler() module from scikit-learn to normalize the data from the CSV file.

-Created a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.
    
-Plotted the data to see what was in the dataframe

![Original Data Graph](https://github.com/margoberry17/19-Crypto-Clustering/assets/136475202/413bfaad-c712-48d4-a35b-f68da1a7d818)


## Found the Best Value for k Using the Original Scaled DataFrame

-Used the elbow method to find the best value for k. Based on the image, 4 is the best value for k.
  
![Elbow Curve](https://github.com/margoberry17/19-Crypto-Clustering/assets/136475202/e63c8d83-b4e9-4611-b52f-9bb63e0be68a)


## Clustered Cryptocurrencies with K-means Using the Original Scaled Data

-Clustered the cryptocurrencies for k=4 on the original scaled data:

![Scatter Plot](https://github.com/margoberry17/19-Crypto-Clustering/assets/136475202/a4668bf1-3372-4b1e-af52-41c75df79267)


## Optimized Clusters with Principal Component Analysis (PCA)

-Using the original scaled DataFrame, I performed a PCA and reduced the features to three principal components.

-Retrieved the explained variance to determine how much information can be attributed to each principal component.

-Created a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.
  

## Found the Best Value for k Using the PCA Data

-Used the elbow method on the PCA data to find the best value for k.

 ![PCA Elbow Curve](https://github.com/margoberry17/19-Crypto-Clustering/assets/136475202/a049330d-0b9e-415f-a3f3-b10e7f0e4735)
 

## Clustered Cryptocurrencies with K-means Using the PCA Data

-Clustered the cryptocurrencies for k=4 on the PCA data.

![CPA Scatter Plot](https://github.com/margoberry17/19-Crypto-Clustering/assets/136475202/8842ca5d-5bc1-4f4f-b5a3-e22fcba8e092)

# Findings

### After comparing the two visualizations it is clear that there was a significant impact of using fewer features since the PCA process condenses features. Both the elbow curves indicated an optimal k-value of 4, yet for the PCA the data is a lot tighter. For both there were two "clusters" that only contained one data point. By implementing PCA and using an optimal k-value of 4 based on the elbow curve, the results were more accurate and percise in clustering the data.

# CryptoClustering
---
### Overview
The project objective was to cluster a group of cryptocurrencies (based on performance) using the K-Means unsupervised learning technique.  

There were several individual deliverables that needed to be completed in order to complete the overall objective:
<ol><li> Prepare the data </li>
    <li> Find the Best Value for k Using the Original Scaled DataFrame </li>
    <li> Cluster Cryptocurrencies with K-means Using the Original Scaled Data </li>
    <li> Optimize Clusters with Principal Component Analysis </li>
    <li> Find the Best Value for k Using the PCA Data </li>
    <li> Cluster Cryptocurrencies with K-means Using the PCA Data </li>
</ol>

### Prepare Data : 
Load [crypto_currency_data](/Resources/crypto_market_data.csv) to a Pandas DF and plot the dataset before transforming
<ul> <li> Use the StandardScaler module to normalize the data.  Note all columns have numeric values </li>
<li> Create a DF with the scaled data -- and set the coin_id column to the column index </li></ul>

### Find the Best Value for k Using the Original Scaled DataFrame: 
I used the elbow method on the scaled dataset determine the best value for 'k'.  
[Elbow Curve - To Determine Optimal Number of Clusters]



### Cluster Cryptocurrencies with K-means Using the Original Scaled Data: 
Once I determined that the optimal value was 4; I trained and predicted the KMeans model using 4 clusters -- and all of the features. The next part of the project used PCA to reduce the number of features


###  Optimize Clusters with Principal Component Analysis: 
I performed a PCA analysis on the original scaled dataframe and reduced the features to 3 principal components.


### Find the Best Value for k Using the PCA Data: 
I used the elbow method on the PCA data to determine the best value for 'k'.  


### Cluster Cryptocurrencies with K-means Using the PCA Data: 
After I determined that the optimal value of clusters was still 4; I trained and predicted the KMeans model; similar to the analysis done on the original scaled dataset.

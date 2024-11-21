# Analysing social pltaform users using machine learning
Utilised supervised learning (Random Forest) and unsupervised learning (K-means) to analyse social platform users behaviour.

### Define the question
Help company understand their customers and provide insight to increase engagement. 

### Exploratory Data Analysis
Examines and visualizes data to understand its main characteristics, identify patterns, spot anomalies, and test hypotheses.
<p align="center">
  <img src="images/EDA1.jpg" alt="Picture 1" width="300"/>
  <img src="images/EDA2.jpg" alt="Picture 2" width="450"/>
</p>
Data transformation (R square/log transformed) is applied after to handle skewness. A correlation matrix is implemented after determine the variables to check the
correlation between variables.<br/>

<p align = 'center'>
<img src="images/correlationPlot.jpg" alt="Correlation plot" width="300"/></p>
<br/>

standardizing or normalizing variables to ensure that each variable contributes equally to the clustering process.

### Unsupervised Model
K-means algorithm partitions a dataset into similar groups based on the distance between their centroids.
Using elbow method to find the optimum number of clusters. Based on EDA part k = 4 in the case.

<p align = 'center'>
<img src="images/Kmeans1.jpg" alt="K-means" width="400"/></p><br/>

silhouette score of 1 denotes that the data point is very compact within the cluster to which it belongs and far away from the other clusters. The worst value is -1. Values near 0 denote overlapping clusters. 
<p align = 'center'>
<img src="images/score.jpg" alt="Silhouette score" width="400"/></p><br/>


Generate insight by analysing clusters respectively. <br/>
Cluster 1 - conversationalists <br/>
Cluster 2 - active users  <br/>
Cluster 3 - quiet readers <br/>
Cluster 4 - information provider <br/>

<p align = 'center'>
<img src="images/result.jpg" alt="Anlysing result" width="400"/></p><br/>


### Supervised Model 
The random forest algorithm is an extension of the bagging method, it  relies on multiple decision trees and accepts the results of the predictions from each tree. Benefit includes resistant to overfitting, presenting estimates for variable importance, handle a wide variety of data types and missing values. <br/>

Split data into training set and test set. <Br/>
Run random forest and tune the hyperparameters. <br/>
<p align = 'center'>
<img src="images/tuning.jpg" alt="Tuning Model" width="400"/></p><br/>


Interpret the result from feature importance. <br/>
<p align = 'center'>
<img src="images/featureImportance.jpg" alt="Feature Importance" width="400"/></p><br/>

Applying confusion matrix to check the classification result. <br/>
<p align = 'center'>
<img src="images/confusionMatrix.jpg" alt="Confusion Matrix" width="250"/></p><br/>


### Analysis and conclusion 

making effort on quiet readers is suggested. More reward mechanisms and interactive communication activities should be strongly encouraged.






# Data-Mining

This repository includes several projects covering different techniques and topics in data mining.  
* [Preprocessing Iris dataset](/IRIS_Preprocessing)
* [Neural Network](/Neural_Network)
* [Association Rules](/Association_Rules)
* [Clustering](/Clustering)
* [Diabetes Classification](/Diabetes_Classifier)

# Preprocessing Iris dataset
The dataset was loaded and preprocessed using pandas and Scikit-learn libraries. Preprocessing steps include dropping null values, normalization and dimensionality  reduction with PCA. The reduced features were visualized using scatter plot and box plot. 

# Neural Network 
## circles classification
In this project, multiple ANNs were trained and fine-tuned to classify a set of randomly generated circles. Each time, different hyperparameters such as activation function, learning rate and number of layers were modified to improve the results. Model loss and accuracy and the final result of each model were plotted. Tensorflow was used as the 

**Final decision boundary plot**

<p align="left">
  <img src="https://user-images.githubusercontent.com/79719208/195886182-988a31ba-153e-4728-80a1-7f96bd8801c3.png" width=39% height=39%>
</p>

## fashion mnist dataset classification
In the second part of the project, a ANN was used for classifying the fashion mnist dataset. 

test accuracy: 0.88

**Confusion matrix**

<p align="left">
  <img src="https://user-images.githubusercontent.com/79719208/195889099-3f826522-8166-4c95-8ff4-e25fec8404a7.png">
</p>

## Association Rules

In this assignment, the apriori algorithm was used to extract association rules in a hypermarket dataset. Three main parameters are support, confidence and lift.


## Clustering

K-means and DBSCAN clustering algorithms were used to cluster data. 

* **K-means**: The elbow method was used to find the optimal value for k. K-means algorithm was also tried on the digits dataset after implementing dimensionality reduction.
* **DBSCAN**: This algorithm performs better on non-linear datasets. KNN was used to optimize epsilon and MinPts value was estimated  through multiple trials.

# Diabetes Classification

As the final project of this course, a classifier was implemented using the XGBoost library and a dataset from Centers for Disease Control and Prevention (CDC) which includes information from more than 70,000 patients. The target column in this dataset is Diabetes_binary which indicates whether a patient has diabetes or not.

* **Preprocessing**
  * dropping binary null values, replacing null numerical features with mean and null categorical features with the most frequent.
  * Normalizing numerical features
  * one-hot-encoding for categorical features
  * Train/test splitting
* A **XGBClassifier** model was trained.
* **GridSearchCV** was used for hyperparameter tuning.

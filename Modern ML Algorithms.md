# Discussion on Modern Machine Learning Algorithms
Machine Learning Algorithms can be categorized as either:
* Generative and Discriminative
* Parametric and Non-Parametric
* Supervised and Unsupervised

There is no one algorithm that works best for every problem. The choice of algorithm should be dependent on factors such as size and structure of the data set. Thus many algorithms should be tried out on a given data set.

## Machine Leanrning Tasks:
* Regression
* Classification
* Clustering

### Regression
A machine learning task is identified as a regression task when our end goal is to predict continuous, numeric values. We have a set of predictors that are used to predict the response. Examples include predicting stock prices, student test scores etc,

There are various regression algorithms that can be used:
* **Linear Regression** - There are various ways of fitting linear regression models
  * Least Squares
  * Lasso
  * Ridge
  * Elastic Net
  The last three ways of fitting basically use the concept of regularization to avoid overfitting.
  
  *Advantages* - Linear Regression in general has high interpretability. This means that the model itself is easy to understand and conclusions about the data set can be obatined from the final model. It also works very well when the data has linear relationship and can be updated when new data comes in using a method called as Stochastic Gradient Descent.
  
  *Disadvantages* - If there exist non-linear relationships in the data, linear regression is not a very wise choice and the predictve accuracy of the model will generally be very poor.
  
* **Regression Trees**
* **Deep Learning**
* **Nearest Neighbors**

### Classification
A machine learning task is identified as a classification task when our aim is to predict categorical variables. Examples include determining whether an applicant should be given a credit card or not, predicting the type of weather etc.

Some popular clasification algorithms are:
* **Logistic Regression**
* **Classification Trees**
* **Deep Learning**
* **Support Vector Machines**
* **Naive Bayes**
* **Linear Discriminant Analysis**

### Clustering
This is basically comes under the domain of unsupervised learning where we do not have labels to our data. Rather the algorithm should do the job of finding patterns in the data set and accordingly allocate data to different clusters.

Some popular clustering algorithms are:
* **K-Means**
* **Gaussian Mixture Models**
* **Affinity Propagation**
* **Hierarchical/Agglomerative Clustering**
* **DBSCAN - Density Based Spatial Clustering of Applications with Noise**



# References
* [Modern Machine Learning Algorithms - Elite Data Science](https://elitedatascience.com/machine-learning-algorithms)


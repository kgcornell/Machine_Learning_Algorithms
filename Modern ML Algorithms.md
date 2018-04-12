# Discussion on Modern Machine Learning Algorithms
Machine Learning Algorithms can be categorized as either:
* Generative and Discriminative
* Parametric and Non-Parametric
* Supervised and Unsupervised

There is no one algorithm that works best for every problem. The choice of algorithm should be dependent on factors such as size and structure of the data set. Thus many algorithms should be tried out on a given data set.

## Curse of Dimensionality
Curse of Dimensionality is a term coined by Richard Bellman and is a group of phenomena associated with high-dimensional data. The underlying theme of all the problems is that when the dimensionality increases, the volume of the space increases so fast that the available data becomes sparse. Let us consider a small example to understand this phenomena (Taken from [Clever Owl](http://cleverowl.uk/2016/02/06/curse-of-dimensionality-explained/). Say we have a data set consisting of 20 training samples and having one feature only. Each of these samples also has an associated label that can be either of the two classes. This means that we are in a binary classification setting. 

Say we divide our sample space into 4 regions and whenever we encounter a new data point, we identify the region to which it belongs and assign it to the class which has the maximum number of data points belonging to it in that region. Lets add one more dimension to our data set. In this scenario, the number of spaces increase from 4 to 16 and the average number of data points in a particular region decreases. Moreover there are regions entirely devoid of data points and our classifier would get confused were it to encounter a data point belonging to these empty regions. This sparsity increases on adding one more dimension as now the number of regions are 64 instead of 16. This is in essence the curse of dimensionality.

Reducing data dimensionality or making the algorithm more robust to high dimensional data are methods for tackling this curse of dimensionality. The former method is more prevalent and the section below analyzes different dimensionality reduction techniques in detail.

## Popular Dimensionality Reduction Techniques
Some of the popular techniques used for this are:

* **Missing Values Ratio**
* **Low Variance Filter**
* **High Correlation Filter**
* **Random Forests/Ensemble Trees**
* **Backward Feature Elimination**
* **Forward Feature Construction**
* **Principal Component Analysis**
* **Linear Discriminant Analysis**
* **Generalized Discriminant Analysis**


With a fixed number of training samples, the predictive power of a classifier/regressor first increases as the number of dimensions increase but then starts decreasing. This is known as *Hughes phenomenon* or *Peaking phenomena*.

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
* **Nearest Neighbors**

### Classification
A machine learning task is identified as a classification task when our aim is to predict categorical variables. Examples include determining whether an applicant should be given a credit card or not, predicting the type of weather etc.

Some popular clasification algorithms are:
* **Logistic Regression**
* **Classification Trees**
* **Support Vector Machines**
* **Naive Bayes**

### Clustering
This is basically comes under the domain of unsupervised learning where we do not have labels to our data. Rather the algorithm should do the job of finding patterns in the data set and accordingly allocate data to different clusters.

Some popular clustering algorithms are:
* **K-Means**
* **Gaussian Mixture Models**
* **Affinity Propagation**
* **Hierarchical/Agglomerative Clustering**
* **DBSCAN - Density Based Spatial Clustering of Applications with Noise**

## No Free Lunch Theorem
This theorem for machine learning states that, averaged over all possible data-generating distributions, every classification algorithm has the same error rate when classifying previously unobserved points. In other words, no machine learning algorithm is universally any better than other.





# References
* [Modern Machine Learning Algorithms - Elite Data Science](https://elitedatascience.com/machine-learning-algorithms)


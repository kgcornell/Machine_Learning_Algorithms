# Naive Bayes Classifier

This classifier works particularly well with Natural Language Processing (NLP) problems.

## Maximum Likelihood Estimation (MLE)
Let us start by understanding what the parameters of a model mean. For a univariate linear regression model given by *y=mx+c*, y is the response, x is the predictor variable while m and c refer to the parameters. MLE is a method for obtaining the values of the parameters of a model. The values are found such that they maximise the likelihood that the process described by the model produced the data that was actually observed. For instance we have some observed data and we believe that this data comes from some probability distribution. Each distribution has parameters that can be used to describe it. For a Gaussian (Normal) distribution, mean and standard deviation are the requisite parameters. MLE will help us in determining these parameters which in turn will give us the entire distribution that maximises the probability of observing the data. 

Thus our aim is to calculate the total probability of observing all the data. Here we need to make some assumptions to simplify the mathematics involved. We assume that the individual data points are generated independently from each other. Therefore the probability of observing the data is given by the multiplication of individual data probabilities. To maximize this probability, we first take log of the expression as log is a monotonically increasing function. We then differentiate the obtained function with respect to the parameters that we want to estimate and set the derivative to 0. This gives us the value of the parameters of the distribution.

**Point to Note**
It is entirely possible that the log-likelihood function might still be analytically intractable. Therefore, iterative methods such as Expectation-Maximization algorithms are used to find numerical solutions for the parameter estimates. 


## References
* [Probability concepts explained: Maximum likelihood estimation - Medium](https://towardsdatascience.com/probability-concepts-explained-maximum-likelihood-estimation-c7b4342fdbb1)

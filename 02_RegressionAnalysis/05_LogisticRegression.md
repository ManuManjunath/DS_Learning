# Logistic Regression
A technique that models a categorical dependent variable (Y) based on one or more independent variables (X)

### Binomial Logistic Regression
A technique that models the probability of an observation falling into one of two categories, based on one or more independent variables.

### Assumptions of Binomial Logistic Regression
* Linearity  
There should be a linear relationship between each X variable and the logit of the probability that Y equals 1.
* Independent Observations  
P(A AND B) = P(A) * P(B)
* No Multicollinearity
* No Extreme Outliers.

$odds = p / (1-p)$  
Odds = Probability of P occuring / Probability of P not occuring.

### Logit (Log odds)
The logarithm of the odds of a given probability. So the logit of probability p is equal to the logarithm of p divided by 1-p.  
$logit(p) = log(p/(1-p))$

### Maximum Likelihood Estimation (MLE)
A technique for estimating the beta parameters that maximize the likelihood of the model producing the observed data.

### Precision
The proportion of positive predictions that were true positives.  
$Precision = True Positives / (True Positives + False Positives)$

### Recall
The proportion of positives the model was able to identify correctly.  
$Recall = True Positives / (True Positives + False Negatives)$

### Accuracy
The proportion of data points that were correctly categorized.  
$Accuracy = (True Positives + True Negatives) / Total Predictions$
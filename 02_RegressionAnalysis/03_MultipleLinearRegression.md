# Multiple Linear Regression
A technique that estimates the linear relationship between one continuus dependent variabe (Y) and two or more independent variables.

#### Equation for Simple Linear Equation
$Y = Intercept + Slope(X)$  
$Y = \beta_0 + \beta_1X$  

#### Equation for Multiple Linear Equation
$Y = Intercept + Slope(X)$  
$Y = \beta_0 + \beta_1X_1 + + \beta_2X_2 + ... + \beta_nX_n$  

#### One Hot Encoding
A data transformation technique that turns one categorical variable into several binary values.  

##### Multiple Linear Regression Assumptions
* Linearity  
Each predictor variable ($X_i$) is linearly reated to the outcome variable (Y)  
To validate this, the data points when plotted, must appear to fall along a straight line.
* Normality  
The residuals or errors are normaly distributed.  
To validate this, a quantile-quantile plot (Q-Q plot) of the residuals can be observed. If the points on the graph appear to fall in a straight diagonal line, then we can assume normality. This can be validatd after the mode is built.
* Independent Observations  
Each observation in the dataset is independent. Ensure there is no auto correlated data in the datasert.
* Homoscedasticity  
The variation of the residuals (errors) is constant or similar across the model. Homoscedasticity means "Having the same scatter". A Scatterplot of residuas and predicted values should form a random cloud.
* No multicollinearity  
No two independent variables ($X_i$ and $X_j$) can be highly correlated with each other.

#### Variance Inflation Factors (VIF)
Quantifies how correlated each independent variable is with all of the other independent variables.  
Minimum value of 1 means there is no correlation between the X variabe and other predictor variables in the model. The larger the VIF, the more multicollinearity there is in the model.

#### How to handle multicollinearity
* Drop one or more variables that have multicollinearity.
* Create a new variable using existing data.

#### Interaction Term
A term that represents how the relationship between two independent variables is assocuated with changes in the mean of the dependent variable.

#### Adjusted $R^2$
A variation of the $R^2$ regression evaluation metric that peanalizes unnecessary explanatory variables.  
Value varies from 0 to 1.

#### $R^2$ vs Adjusted $R^2$
* Adjusted $R^2$ is used to compare models of varying complexity.
* Determines if you should add another variable or not.
* $R^2$ is more easily interpretable.   
* Determines how much variation in the dependent variable is explained by the model.

#### Underfitting
In the case of underfitting, a multiple regression model fails to capture the underlying pattern in the outcome variable. An underfitting model has a low $R^2$ value.  
A model can underfit the data for a variety of reasons. The independent variables in the model might not have a strong relationship with the outcome variable. In this situation, different or additional predictors are needed. It could be the case that the sample dataset is too small, and this prevents the model from being able to learn the relationship between the predictors and the outcome. Using more sample data to build the model might reduce the problem of underfitting.

#### Overfitting
When a model fits the observed or training data too specifically, and is unable to generate suitable estimates for the general population.

#### Bias-Variance trade off
Balance between two model qualities, bias and variance, to minimize overall error for un-observed data. 

Bias simplifies the model predictions by making assumptions about the variable relationships.  
A highly biased model may oversimplify the relationship, underfitting to the observed data, and generating inaccurate estimates. 

Variance in a model allows for model flexibility and complexity, so the model can learn from existing data. But a model with high variance can overfit to observed data and generate inaccurate estimates for unseen data.

#### Holdout Sampling
The sample data intois divied two categories called training data and test data. Training data is used to build the model, and test data is used to evaluate the model’s performance after it has been built. Splitting the sample data in this way is called holdout sampling, with the holdout sample being the test data.  
Holdout sampling allows data scientists to evaluate how a model performs on data it has not experienced yet.

#### Feature Selection
Also known as Variable Selection is the process of determining which variables or features to include in a given model.

#### Forward Selection and Backward Elimination
Forward Selection is a stepwise variable selection process that begins with the null model, with 0 independent variables, considers all possible variables to add.  
It incorporates the independent variable that contributes the most explanatory power to the model.

Backwards Elimination is a stepwise variable selection process that begins with the full model, with all possible independent variables, and removes the independent variable that adds the least explanatory power to the model.

#### Extra Sum of Squares F-test
Quantifies the difference between the amount of variance that is left unexplained by a reduced model that is explained by a full model. 

## Reguarization
A set of regression techniques that shrinks regression coefficient estimates toward zero, adding in bias, to reduce variance.

#### Regularized Regression Techniques
* Lasso Regression
* Ridge Regression
* Elastic-net Regression
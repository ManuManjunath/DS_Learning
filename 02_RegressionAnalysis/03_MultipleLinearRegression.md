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
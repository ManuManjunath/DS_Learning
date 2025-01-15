# Simple Linear Regression
A technique that estimates the linear relationship between one independent variable (X) and one continuus dependent variabe (Y)

##### Equation
$Y = Intercept + Slope(X)$  
$Y = \beta0 + \beta1X$  

##### Best fit line
There could be many different lines that might fit the data. However, we need to find the best fit line.  
The line that fits the data best by minimizing some loss function or error.

##### Predicted Values
The estimated Y values for each X calculated by a model.

##### Residual
The difference between observed or actual values and the predicted values of the regression line.  
$Residual = Observed - Predicted$  
$\epsilon_i = y_i - y*_i$

##### Sum of Squared Residuals
The sum of squared differences between each observed value and its associated predicted value.  
$\sum(Observed-Predicted)^2$

##### Ordinary Least Squares (OLS)
A method that minimizes the sum of squared residuals to estimate parameters in a linear regression model.

##### Correlation
Correlation is a measurement of the way two variables move together. If there is a strong correlation between the variables, then knowing one will be very helpful to predict the other. However, if there is a weak correlation between two variables, then knowing the value of one will not tell you much about the value of the other.  

The Correlation Coefficient (r)  quantifies the strength of the linear relationship between two variables. It always falls in the range of [-1, 1]. When r is negative, there is a negative correlation between the variables: as one increases, the other decreases. When r is positive, there is a positive correlation between the variables: as one increases, so too does the other. When r = 0, there is no linear correlation between the variables.

The closer r is to -1 or 1, the more linear the data appears. When r is exactly 1 or exactly -1, then the variables are perfectly correlated, and their graph is a line. When r is zero, there is no correlation between the variables, and the data appears as a shapeless cloud of points. 

##### Linear Regression Assumptions
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

# Model Evaluation

#### Confidence Band
The area surrounding the line that describes the uncertainity around the predicted outcome at every value of X.

#### Common Evaluation Metrics
* $R^2$ (Co-efficient of determination)
* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)

#### $R^2$
Measures the proportion of variation in the dependent variable (Y), explained by the independent variables (X).  
If $R^2$ = 1, it means X explains 100% of the variance of Y.  
A higher $R^2$ is better since it adds validity to any recommendation we make based on our analysis.

#### MSE
It is the average of the squared difference between the predicted and actual values.  
Because of how MSE is calculated, MSE is very sensitive to large errors.

#### MAE
It is the average of the absolute difference between the predicted and actual values.  
If your data has outliers that you want to ignore, you can use MAE, as it is not sensitive to large errors.

#### Hold-out sample
A random sample of observed data that is not used to fit the model.
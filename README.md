# Linear-Regression
Linear Regression example

- ## Assumptions of Linear Regression
  #### 1. The regression model is linear in the coefficients and the error term
  - This assumption addresses the functional form of the model. In statistics, a regression model is linear when all terms in the model are either the constant or a parameter multiplied by an independent variable. Y = mx + b
 
  #### 2. The error term has a population mean of zero
  - The error term accounts for the variation in the dependent variable that the independent variables do not explain. Random chance should determine the values of the error term. For your model to be unbiased, the average value of the error term must equal zero.

  - Suppose the average error is +7. This non-zero average error indicates that our model systematically underpredicts the observed values.

  ####  3. All independent variables are uncorrelated with the error term
  - If an independent variable is correlated with the error term, we can use the independent variable to predict the error term, which violates the notion that the error term represents unpredictable random error.

  ####  4. Observations of the error term are uncorrelated with each other
  - One observation of the error term should not predict the next observation.
  
  -  If you have information that allows you to predict the error term for an observation, you need to incorporate that information into the model itself.
  
  #### 5. The error term has a constant variance (no heteroscedasticity)
  - The variance of the errors should be consistent for all observations. In other words, the variance does not change for each observation or for a range of observations. This preferred condition is known as homoscedasticity (same scatter). If the variance changes, we refer to that as heteroscedasticity (different scatter).

  - The easiest way to check this assumption is to create a residuals versus fitted value plot. On this type of graph, heteroscedasticity appears as a cone shape where the spread of the residuals increases in one direction. In the graph below, the spread of the residuals increases as the fitted value increases.
  
    ![Image description](https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2017/08/residuals_unfixed.png?w=576&ssl=1)

  - Residuals by fitted values plot that displays heteroscedasticity, which violates an OLS assumption.
  
  #### 6. No independent variable is a perfect linear function of other explanatory variables
  - Perfect correlation occurs when two variables have a Pearson’s correlation coefficient of +1 or -1. When one of the variables changes, the other variable also changes by a completely fixed proportion. The two variables move in unison.
  
  #### 7. The error term is normally distributed (optional)
  - OLS does not require that the error term follows a normal distribution to produce unbiased estimates with the minimum variance. However, satisfying this assumption allows you to perform statistical hypothesis testing and generate reliable confidence intervals and prediction intervals.

- The easiest way to determine whether the residuals follow a normal distribution is to assess a normal probability plot. If the residuals follow the straight line on this type of graph, they are normally distributed. They look good on the plot below!
  ![Image description](https://i0.wp.com/statisticsbyjim.com/wp-content/uploads/2018/05/normal_probability_plot_residuals.png?w=576&ssl=1)
  
https://statisticsbyjim.com/regression/ols-linear-regression-assumptions/


- ## Definitions
  ####  Dependent variable
  - The value you want to predict
  - The y value
  
  #### Independent variable 
  - Each parameter given as input to the model can be called an independent variable
  - Also known as the x values or predictors
  
  #### R squared
  - Determines how well your model can predict the dependent variable
    
  #### Null hypothesis
  - States that the model with no independent variables fits the data as well as your model
   
  #### F-test
  - Tests if your model has statiscal significant or fits the null hypothesis
  
  #### Significant value
  - The probability of rejecting the null hypothesis. This value is usually 0.05 or 5%.
  
  #### P-value
  - Determines the statistical significance of each independent variable. A P value < the the signicant value means that the independent variable has statistical significance. 
  
  #### Coeficients
  - The coeficient for an independent variable determines the rate of change for the dependent variable. Meaning that a coeficient of 2 for a variable x will change y by 2x for every unit in change of x (y = 2x) .

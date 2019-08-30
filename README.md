# Machine-Learning-on-R

# Task A: Linear Regression
Build a linear regression model using the specific “auto mpg train.csv” provided with the assignment to predict mpg (mile per gallon). The second file “auto mpg test.csv”will be used for evaluation.

`Data Set Information: The data concerns city-cycle fuel consumption in miles per gallon, to be predicted in terms of 3 multivalued discrete and 5 continuous attributes.`
1. mpg: continuous, target variable 
2. cylinders: multi-valued discrete 
3. displacement: continuous 
4. horsepower: continuous 
5. weight: continuous 
6. acceleration: continuous 
7. model year: multi-valued discrete 
8. origin: multi-valued discrete 
9. car name: string (unique for each instance)

* Task A.1: There are some missing values listed as “?”. Describe your strategy for treating missing values and update (edit by hand) the file accordingly.
* Task A.2: Pair plot mpg vs. the other variables to visualize the relationships and discuss what you see.
* Task A.3: Based on your pair plots, propose an initial set of variables to use for a multiple linear regression model to predict mpg.
* Task A.4: With variables of your choice build the model using the lm() routine in R, and then print the summary of the model to get the R diagnostics. Briefly explain the statistics in the summary, e.g. R2 value, t-value, standard error, p-value (ignoring the F-statistics line). What does this imply about the predictors for your model?
* Task A.5: Test the fitted model using the “auto mpg test.csv”, and calculate the MSE on the test set, reporting it. Note the test set has no missing values.
* Task A.6: Can you improve your model with different predictors? Try out some different ratios or products of the better predictor variables. How will you evaluate the different alternative predictors on your existing model (not using the test set)? Evaluate them and suggest which single predictor you would like to add (or none, if it looks like none would improve it). If you suggest adding a single predictor, then add it and repeat step A.5 to evalute it on the test set.

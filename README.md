# Machine-Learning-on-R

What you fill find in the rmarkdown file ?

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


# Task B: Logistic Regression
Build a logistic regression model using the specific “adult income train.csv” provided with the Assignment to predict the income variable. The second file “adult income test.csv”will be used for evaluation.

`Data Set Information: Details of the dataset is available at http://www.cs.toronto.edu/ delve/data/adult/. `

Attribute information:
1. age: continuous 
2. workclass: multi-valued discrete
3. fnlwgt: continuous 
4. education: multi-valued discrete 
5. educational-num: continuous 
6. marital-status: multi-valued discrete 
7. occupation: multi-valued discrete 
8. relationship: multi-valued discrete 
9. race: multi-valued discrete
10. gender: binary discrete 
11. capital-gain: continuous 
12. capital-loss: continuous 
13. hours-per-week: continuous 
14. native-country: multi-valued discrete 
15. income: binary discrete

* Task B.1: There are some missing values listed as “?”. Describe your strategy for treating missing values, but note sometimes it is OK to leave missing value as a separate categorical value (we call this “missing informative”). Note there are too many to edit by hand, so if you wish to modify them, identify them with a Boolean test like data$workclass[id]==’?’
and modify the values in a loop.
* Task B.2: With all variables, build a model usingthe glm(income∼.,family=binomial, data=???)
routine in R, and then print the summary of the model to get the R diagnostics. Briefly explain the statistics in the summary, e.g. Z-value, standard error, p-value. What does this imply about the predictors for your model? Notice many of the variables are multi-valued categorical, and in most cases only some of the values are significant.
* Task B.3: Test the fitted model using the “adult income test.csv”, and calculate the confusion matrix on the test set, reporting it. Also, give the precision, accuracy and recall (Lecture 3). Note the test set has no missing values.
* Task B.4: Can you improve your model with different predictors? For instance, you might reconstruct the categorical features to only include significant values and then have an “other” value that groups together all non-significant ones. Perhaps the best way to do this is to create a new data frame with your modified attributes and build the model on that using the R construct “income∼.” Report the R diagnostics and the confusion matrix and other scores on the test set (as per B.3) for the new model and comment on the difference.

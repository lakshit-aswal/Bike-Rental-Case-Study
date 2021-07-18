Conclusions based on analysis:

1)	The following points were made from the dependence of target variable on categorical variables:
  i)	The analysis has shown that, during summer and fall season, the rental count is more compared to spring and winter.
  ii)	The year 2019 has gathered more rentals than the previous year.
  iii)	On holidays, the average rental is less compared to non-holiday.
  iv)	Almost every weekday has same average rental count.
  v)	September and October months has seen better rentals compared to others.

2)	When we create dummy variables for a categorical variable, we use n-1 categories.
So we provide “drop_first = True” parameter to the function, which ignores one category and creates n-1 dummy variables, which leads to less correlation between predictors.

3)	“temp” and “atemp” columns have decent correlation with the target variable but so does the “casual” and “registered” columns, but they are to be ignored as they build the target variable itself.

4)	After building the model on training set, we can see through the summary that the r-squared value of the model is quite decent (around 0.82), and also, we see the p-values of the predictors which were less that 0.05, hence we validate the assumptions of the Linear Regression.
Also, the residuals having a normal form, is also a factor to validate the assumptions.

5)	Year, temperature and winter columns were the better features contributing towards the demand.

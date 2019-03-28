# Hours_Spent_On_Labs_Survey
DSCI 554 Survey Design and Experiment Study

###

6. From 1 to 5, rate your statistical knowledge.

> A student with better statistical knowledge is less likely to go to office hour and spend less time on labs since this student is more likely to understand the concepts well.  

7. Do you do optional questions?

> If a student decides to do optional questions, this student probably understands the material well, and thus they are less likely to go to the office hour. Given the fact thet this student is doing optional questions, the hours this person spend on labs will increase.


### Analysis Plan

We plan to use regression with log transformation to analyze the survey results. 

Before employ our regression model, we plan to do exploratory data analysis first. We will look at our survey results and deal with outliers, such as removing them, at this stage.

Our response variable is expected to be bounded between 0 and 168 hours. Since our response variable, average hours spend on labs, is non-negative, we decide to apply log transformation for normality. The formula for our regression is specified as the following:

$$Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \beta_3 X_3 + \beta_4 X_4 + \beta_5 X_5 + \beta_5 X_5 + \beta_6 X_6 + \beta_7 X_7$$



 
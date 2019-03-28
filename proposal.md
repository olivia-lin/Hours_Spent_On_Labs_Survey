# Hours_Spent_On_Labs_Survey
DSCI 554 Survey Design and Experiment Study

### Analysis Plan

We plan to use regression with log transformation to analyze the survey results. 

Before employ our regression model, we plan to do exploratory data analysis first. We will look at our survey results and deal with outliers, such as removing them, at this stage.

Our response variable is expected to be bounded between 0 and 168 hours. Since our response variable, average hours spend on labs, is non-negative, we decide to apply log transformation for normality. The formula for our regression is specified as the following:

$$Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \beta_3 X_3 + \beta_4 X_4 + \beta_5 X_5 + \beta_5 X_5 + \beta_6 X_6 + \beta_7 X_7 + \beta_8 X_8$$



 
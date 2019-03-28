# Hours_Spent_On_Labs_Survey
DSCI 554 Survey Design and Experiment Study

This survey will investigate the following question:

How does the number of times someone goes to office hours affect the average number of hours a Master of Data Science student spends working on labs per week?

# Confounding Variables

We will address the confounding variables with the following questions:

1. Do you work in groups or alone?

  > Someone working in groups may have enough support to complete labs without going to office hours, but at the same time, someone working in groups may spend more time on labs due to spending time on discussions.

  Working in groups is a confounding variable because the time spent working on labs can decrease when working in groups compared to working alone and affect whether someone attends office hours or not.

2. What is your academic background (i.e. Science, engineering, math, business or other)?

  > Since MDS courses are heavily statistics and computer science based, someone with a statistics or computer background are less likely to go to office hours and more likely to spend less time on labs.

3. How many years have you been out-of-school?

  > The longer someone has been out-of-school, they are less likely to be used to the school routine and may struggle more academically. Therefore, the longer someone has been out-of-school, the more likely someone will go to office hours and the more time someone will spend on labs.

4. From 1 to 5, rate your programming skills.

  > The amount of time an MDS student spends on lab might not only be affected by their understanding of the concepts but also by their ability to translate their understanding into code.  A student with strong programming skills might be efficient at the latter and spend less time on labs. At the same time this student might be less likely to need any help with coding, hence less likely to go to office hours.

5. From 1 to 5, rate your statistical knowledge.

  > A student with strong statistical knowledge will more likely understand concepts of certain MDS courses more quickly and spend less time on labs. At the same time, this student may require less help with concepts, hence less likely to go to office hours.

6. From 1 to 5, rate your statistical knowledge.

  > A student with better statistical knowledge is less likely to go to office hour and spend less time on labs since this student is more likely to understand the concepts well.  

6. Do you do optional questions?

  > If a student decides to do optional questions, this student probably understands the material well, and thus, less likely to go to the office hour. On the other hand, given the fact that this student is doing optional questions, the hours this person spend on labs will increase.

### Analysis Plan

First, we plan to do exploratory data analysis to explore our survey results and deal with outliers, such as negative values or out-of-bound values by removing them.

Next, we plan to do regression with log-link transformation to analyze the survey results because our response variable is expected to be positive. Our response variable is expected to be bounded between 0 and 168 hours. The formula for our regression is:

![](imgs/Proposal_eq.PNG)

Finally, we will determine how office hours affect average time spent on labs per week by interpreting \beta_1 while holding all other variables constant. On average, one time increase in office hours is expected to increase hours spent on labs per week by exp(\beta_1) times.

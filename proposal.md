# DSCI 554 Survey Design and Experimental Study

This survey will investigate the following question:

How does the number of times a Master of Data Science (MDS) student goes to office hours affect the average number of hours they spend working on labs per week?

## Confounding Variables

Confounding variables in our study include whether someone works on labs in groups or alone, someone's academic background, the number of years someone has been out-of-school, someone's competency in programming and statistics and whether someone attempts optional questions. We will address the confounding variables with the following questions and provide explanations for why these variables are confounding under each question:

1. Do you work in groups or alone?

  > Someone working in groups may have enough support to complete labs without going to office hours, but at the same time, someone working in groups may spend more time discussing lab questions and thus spend more time on labs.

2. What is your academic background (i.e. Science, engineering, statistics, math, business, arts or other)?

  > Since MDS courses are heavily statistics and computer science based, someone with a statistics or computer science background are less likely to go to office hours. Furthermore, someone with a statistics or computer science background are more likely to finish labs faster because they are more rehearsed in the topics covered by the MDS curriculum.

3. How many years have you been out-of-school?

  > The longer someone has been out-of-school, the more likely for them to not be used to school routines and thus, more likely to struggle academically. Therefore, the longer someone has been out-of-school, the more likely someone will go to office hours to ask for help. At the same time, this student may not go to office hours, but spend more time on labs just because they are struggling.

4. From 1 to 5, rate your programming skills.

  > The amount of time an MDS student spends on lab might not only be affected by their understanding of the concepts but also by their ability to translate their understanding into code.  A student with strong programming skills might be efficient at the latter and spend less time on labs. At the same time this student might be less likely to need any help with coding, hence less likely to go to office hours.

5. From 1 to 5, rate your statistical knowledge.

  > A student with strong statistical knowledge might understand concepts of certain MDS courses more quickly and spend less time on labs. At the same time, this student may require less help with concepts, hence less likely to go to office hours.

6. Do you do optional questions?

  > A student who decides to solve optional questions probably understands the material well, and thus, is less likely to go to office hours. On the other hand, compared to a person who only do mandatory questions, this student might spend more time working on labs.

## Statistical Analysis

**Null hypothesis:** The number of times a MDS student attends office hours does not affect the average number of hours spent working on labs per week?

**Alternative hypothesis:** The number of times a MDS student attends office hours affects the average number of hours spent working on labs per week?

#### Plan:

First, we plan to do exploratory data analysis to explore our survey results and deal with outliers, such as negative values or out-of-bound values by removing them.

Next, we plan to analyze the survey results using regression with a log-link transformation because our response variable is expected to be non-negative. Our response variable is expected to be bounded between 0 and 168 hours (i.e maximum hours per week). The formula for our regression is:

![](imgs/Proposal_eq.png)

Finally, we will determine how office hours affect average time spent on labs per week by interpreting *β*<sub>1</sub> while holding all other variables constant. On average, one visit increase in office hours is expected to increase hours spent on labs per week by *e*x*p*(*β*<sub>1</sub>) times.

## Online Surveys Ethics

Our proposed survey is not collecting any direct identifying information (including IP address). It is only collecting one indirect identifier in survey Question 2, which is the academic background of the respondent. It would be very difficult to re-identify the respondents from this piece of information.

As our study is limited to the online survey, a cover letter will be presented to the participant for them to make an informed decision about participating in the survey study. We will use a Canadian-hosted survery tool and all survey data will be stored and accessed in Canada only.

The survey will comply with BC Freedom of Information and Protection of Privacy Act (FIPPA). For more details, please see [UBC Office of Research Ethics document on Using Online Surveys](https://ethics.research.ubc.ca/sites/ore.ubc.ca/files/documents/Online_Survey-GN.pdf).

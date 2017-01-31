### ***Project 1 Feedback***

***Nico Van de Bovenkamp***
***

**Overall:** Great work! You answers are well structured, and very inline with how you should be approaching these problems -- very thorough!

**Some Notes**

I actually don't think that this data is randomly generated? But I am not sure. It comes from UCLA's department of statistics. You can look up their lesson online, which will actually provide some insight into building the logistic regression on this data.

* ***Part 2 - Q.3a:*** You are definitely right, the mean is sensitive to outliers and has the potential to bust part of your analysis/model. However, the 'median' is actually more robust to outliers. Although more data can shift the mean, we usually don't see the median effected by outliers.

**Something to think about:**
    We don't touch on it too much in class, but think about how you can apply statistical tests to your data. There are many handy tests to determine difference of means (very useful), tests to determine assumptions of an underlying distribution, etc.

**Bonus notes** You can use a linear regression model for this problem that takes on that structure, but you would actually be making use of a probit model. In this case, you will be calculating probability density of a student being admitted or not admitted P(admitted | gre,prestige,gpa). Another choice of a basic, linear model would be a Logistic Regression. Let me know if you would like more info here, but we will see model building soon!

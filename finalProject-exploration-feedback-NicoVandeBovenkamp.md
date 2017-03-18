### ***Final Project - Exploratory Analysis Feedback***

***Nico Van de Bovenkamp***
***

**Overall:** This notebook is a great start to working with your dataset, cleaning some stuff up, and gaining some insight! And good work creating those methods to be applied to your dataset!

**Analysis Structure:** Overall, the biggest step is going to be deciding what features to use, impute, and drop. Once that is done, you will build your classifier(s!) on is_late! Models learn exceptionally differently, so I would try for something linear (a Logistic Regression with Statsmodels API for some more statistical insight and/or a linear SVM), then move on to non-linear models (Random Forrest, Gradient Boosted Trees, etc.).

**Some thoughts and notes:**

* **Plot Styling:** Ggplot works/looks solid, but I found out that someone made a FiveThirtyEight matplotlib styling that is very cool!
* **Missing Values:** With features that have tons of missing values, you're likely to just lose them all together. For the ones that don't have as many missing values, you can potentially impute the means and gain a lot more out of your data.
* **Model Tuning:** Always remember your Train/Test Split, Regularization, Cross-Validation, Visualizing learning paths, etc.
* **Base Rates:** In this analysis, you have a higher proportion of on-time payments than ones that are late. Thus, you will have to be mindful with the metrics, and thresholds, your models are using because a model might seem to perform well, but it could just be predicting the On-Time consistently (which is not very useful!). Also, we didn't really discuss this, but you could make use of some down-sampling scheme to make the classes more even.
* **Scaling Data:** Check out the [Standard Scaler](http://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html) package. The Standard Scaler will scale all numerical data, which will allow for some easier computation and more efficient computation. This part can actually be quite critical for distance based functions and SVMs.
* * **Feature Importance:** One nice feature of random forests, is the ability to use, and then plot, the `.feature_importance_` of each feature (usually calculated via minimal entropy or gini coeffient). In These types of *why and what factors influence [blank]* problems, the prediction power of a feature can be very handy!

***A Table of Key Evaluation Metrics and Visuals:***

*Throwing this in here too! Below is a brief set of many ways you can communicate/measure results that will be useful for your final project. Please let me know if you have any questions!*

| Metrics | |
|--- | --- |
| *Classification* | Accuracy, Precision, Recall, AUC Score, Lift, F-Score, Log-Loss, Gini, Entropy/Information Gain, Statistical Significance (p-value) |
| *Regression* | Mean Squared Error, Mean Absolute Error, Log-Likelihood Estimation, Statistical Significance (p-value) |

| Visualizations | |
|--- | --- |
| *Model Tuning* | Learning Curves, Regularization Learning Paths with an Error Metric, Model Error stepwise increasing feature set size |
| *Classification* | ROC Curve, Feature Importance Charts, Lift Curves, Expected Value Plots |
| *Regression* | Residual plots(!), KDE and KDE of Predicted Values, Expected Value |

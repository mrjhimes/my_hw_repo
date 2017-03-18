### ***Project 4 Feedback***

***Nico Van de Bovenkamp***
***

**Overall:** Nice work on this final notebook! Your discussion and write up is very thorough, and to the point, which will pay off when you are doing this for your final project. Regarding further exploration, you have some awesome points of focus looking ahead. The one note I would make on look forward: include different models and different methods of investigating current data!

**Some thoughts:** I noticed that you dropped the missing values, which is fine as there are not many, but if you can test the missing values (via a difference of means test), imputing the means may be a bit better as to not lose out on valuable instances! Also, given you used Statsmodels API, you could talk about the statistical significance (p-values) for each coefficient (feature, in Machine Learning).  ***As always, try out many different models!***

**Other Visualizations:** In your final presentation, it is often hard to find the best way to show your results. Sometimes, it is in just bits of code or sudo-code, but often we want clean images and visualizations. The predicted probabilities (which works in the case of classification) across several values provided are one fantastic way of conveying results. However, think back to the lectures were we show learning curves, ROC curves, and discuss many error metrics. Showing those error metrics, and some visualizations of how you control or tune models to impact an evaluation metric is key! Think about this for your final project.

***A Table of Key Evaluation Metrics and Visuals:***

*Below is a brief set of many ways you can communicate/measure results that will be useful for your final project. Please let me know if you have any questions!*

| Metrics | |
|--- | --- |
| *Classification* | Accuracy, Precision, Recall, AUC Score, Lift, F-Score, Log-Loss, Gini, Entropy/Information Gain, Statistical Significance (p-value) |
| *Regression* | Mean Squared Error, Mean Absolute Error, Log-Likelihood Estimation, Statistical Significance (p-value) |

| Visualizations | |
|--- | --- |
| *Model Tuning* | Learning Curves, Regularization Learning Paths with an Error Metric, Model Error stepwise increasing feature set size |
| *Classification* | ROC Curve, Feature Importance Charts, Lift Curves, Expected Value Plots |
| *Regression* | Residual plots(!), KDE and KDE of Predicted Values, Expected Value |

This [R analysis](https://github.com/bdavidson16/R/blob/main/House%20Price%20Predictions/House%20Price%20Predictions%20MAT%20303%20Project.ipynb) focuses on housing features and how they affect the price. We use regression models and a nested F-test to not only find out which features of a house affect the price the most, but to also find out which model is best to use in this situation.

*Why*?

Home buyers and sellers can accurately negociate offers. Real estate agents can understand the houses they are selling and looking for. As well as government officials can use this information to form policies on housing assistance. There are so many more uses with this informaiton.
# [Data]():


# Outline of [Summary Report]():
- Intro
- Data Prepping
- Model 1: First Order Regression
- Model 2: Second Order Regression
- Nest Models F-Test
- Conclusion

# Concluding Points
Which model is best?
- I would choose the complete second order regression model with quantitative variables.
  - I would choose the complete over the reduced because it is significantly better based on the nested F-tests completed.
  - I would choose the second order regression model over the first order because the predictors, in this case the features, do not have a perfect linear relationship to the outcome, the price.
- The adjusted R for the first order model is 0.6029, which means that only 60% of the values are explained by the model.
- The second order model has a percentage of almost 81%. Even though the variables are different, each variable in both models have individual significance on a house’s price.
- Also, the first order model has more significant variables than the second order, so it should have a higher adjusted R-squared.
- However, the second order model is just a better fit and I recommend to use this one for better predictions of house prices.

<ins>Model 1:</ins>

The variables that are significant at 5% are the living area (sqft), upper-level area, age, bathrooms, view1, and view2, because they all have a p-value less than 0.05 and their t-values are not close to the mean, specifically more than 2. In addition to not including zeros in their confidence intervals. This means that we reject the null hypothesis and can say that for every change in each of these features, the price of a house is significantly affected.

<ins>Model 2:</ins>

All of the variables are significant at 5% besides the School Rating:Crime interaction term, which is close to the mean and has a high p-value. The variables that are significant also do not include zeros in their confidence intervals. Therefore, we can reject our null hypothesis and conclude that all of these housing features in this model, besides the interaction term between School Rating and Crime, have a significant effect on the price of a house. In other words, when a housing feature changes it can significantly change the price of that house.


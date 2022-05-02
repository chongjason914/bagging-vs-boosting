# Battle of the Ensemble - Random Forest vs Gradient Boosting 

## Introduction
This repository aims to explore the difference between two ensemble methods: bagging (random forest) and boosting (gradient 
boosting). 

Ensemble methods involve aggregating multiple machine learning models with the aim of decreasing both bias and variance. Ideally,
the result from an ensemble method will be better than any individual machine learning model. 

## Bagging
Bagging, also known as bootstrap aggregating, refers to the process of creating and merging a collection of independent, parallel
decision trees using different subsets of the training data (bootstrapped datasets).

Decision trees built using random forest have zero knowledge and influence on the other trees in the model. Once all the trees 
are built, the model will then select the mode of all the predictions made by the individual decision trees and return the
result as the final prediction.

In summary, random forests:
- Create independent, parallel decision trees
- Work better with a few, deep decision trees
- Have a short fit time but a long predict time

## Boosting
Boosting, on the other hand, takes an iterative approach to combine a number of weak, sequential models to create one strong model
by focusing on the mistakes in the prior iterations.

A weak model is one that is only slightly better than random guessing whereas a strong model is one that is strongly correlated
with the true classification.

In summary, gradient boosting:
- Builds trees in a successive manner where each tree improves upon the mistakes made by previous trees
- Works better with multiple, shallow decision trees 
- Have a long fit time but a short predict time

## Medium article
For a more detailed explanation on this topic, check out the full article on Towards Data Science [here](https://towardsdatascience.com/battle-of-the-ensemble-random-forest-vs-gradient-boosting-6fbfed14cb7).

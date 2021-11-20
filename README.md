# Ensemble-Methods-in-Machine-Learning 
 
 ### Bagging: 
 
Bagging is a technique for merging the outputs of various models (for example, all decision trees) to produce a more generic result. Here's a question for you: Will it be useful if you develop all the models on the same set of data and integrate them? Given the same input, there's a good likelihood that these models will produce the same outcome. So, what are our options for resolving this issue? Bootstrapping is one of the techniques.

Bootstrapping is a sampling method that involves replacing subsets of observations from the original dataset. The size of the subsets is equal to the original set's size.

These subsets (bags) are used in the Bagging (or Bootstrap Aggregating) technique to acquire a good picture of the distribution (complete set). The size of the bagging subsets may be smaller than the original set.

![image](https://user-images.githubusercontent.com/86415241/142719223-cd2a0668-2e0a-41bb-ada9-b5a001b805ec.png)


1. From the original dataset, many subsets are formed by replacing observations.
2. On each of these subsets, a basic model (weak model) is generated.
3. The models are independent of one another and run in parallel.
4. The final predictions are determined by merging all of the models' projections.

![image](https://user-images.githubusercontent.com/86415241/142719228-2231b343-10c4-46b6-be44-01c38c4e366f.png)



### Boosting

Boosting is a sequential procedure in which each successive model seeks to rectify the prior model's mistakes. The models that follow are dependent on the prior model. Let's have a look at how boosting works in the steps below.

1. A subset is created from the original dataset.
2. Initially, all data points are given equal weights.
3. A base model is created on this subset.
4. This model is used to make predictions on the whole dataset
5. Errors are calculated using the actual values and predicted values.
6. The observations which are incorrectly predicted, are given higher weights.
7. Another model is created and predictions are made on the dataset.
8. Similarly, multiple models are created, each correcting the errors of the previous model.
9. The final model (strong learner) is the weighted mean of all the models (weak learners).



#### Bagging algorithms:
- Bagging meta-estimator
- Random forest


#### Boosting algorithms:
- AdaBoost
- GBM
- XGBM
- Light GBM
- CatBoost

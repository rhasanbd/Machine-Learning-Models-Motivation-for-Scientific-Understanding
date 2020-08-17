# Machine Learning Classifier Models: Justification for Scientif Understanding

In this repository we address the following question:

- Given a problem (dataset), how do we choose the best ML model and its settings?

More specifically, we emphasize the need for acquiring a scientific understanding of the ML models. Lack of this knowledge limits our ability to use ML for solving practical problems in two ways:
- We don't know how to select the best model
- We don't know how to find optimal hyperparameters of a chosen model

Due to this knowledge gap we resort to the brute-force techniques of trying every possible ML model and search over every possible combination of the hyperparameter values. This is not science, and nor is it feasible for large and complex problems.

In this notebook we will explore 10 Machine Learning (ML) classifier models:
1. K-Nearest Neighbor (KNN)
2. Logistic Regression
3. Polynomial Logistic Regression
4. Naive Bayes
5. Linear Support Vector Machine (Linear SVM)
6. Non-Linear Support Vector Machine (SVM Gaussian Radial Basis Function)
7. Decision Tree
8. Ensemble Method: Random Forest
9. Ensemble Method: Voting Clasifier
10. Multi-Layer Perceptron (MLP)




We will use the Scikit-Learn implementations of these models and compare their performance on a two-dimensional and non-linear synthetic dataset. Thus, the models will be used to solve a **binary classification problem**.

We will split the dataset (randomly) into training and test subsets, then train each model using the training data subset. Finally, we will evaluate a model's performance on the unseen test data subset.

The performance of each model depends of a set of parameters or hyperparameters. The standard practice in ML is to first find the optimal hyperparameters by searching over a range of values for the hyperparameters. This technique is known as hyperparameter tuning. Unless the optimal hyperparameter values are selected in training a model, it will not perform optimally. 

In this notebook we will not exhaustively search optimal hyperparameters. In most of the cases we will use the Scikit-Learn default setting of the hyperparameters. However, we may vary only a few key hyperparameters to show how they influence the model's performance on test data.

We will see that most of the models are very sensitive to the choice of hyperparameter values. Thus, it is imperative to learn how to choose hyperparameters optimally. Also not all models are equally effective for a given dataset. A deep knowledge on the models is essential for finding the best model.


## Takeaway Lesson

There are at least two takeway lessons:

- 1. The problem (dataset) should dictate the choice of models. It's never a good idea to search over every possible model.

- 2.  While an informed hyperparameter tuning is useful for smaller datasets, a blind and brute-force search over the hyperparamter space is never a good idea, because:

      -- It's not science.
      
      -- It's not feasible for complex models such as MLP that uses very large dataset.


Thus, after reviewing this notebook we should be able to convince ourselves **the need for acquiring a scientic understanding of these ML models**, which will lead toward the knowledge on optimal training of the models.

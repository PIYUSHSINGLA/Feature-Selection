# Feature Selection 

Feature Selection is one of the core concepts in machine learning which hugely impacts the performance of your model. The data features that you use to train your machine learning models have a huge influence on the performance you can achieve.

Irrelevant or partially relevant features can negatively impact model performance. Therefore, Feature selection and Data cleaning should be the first and most important step of your model designing.

Feature Selection is the process where you automatically or manually select those features which contribute most to your prediction variable or output in which you are interested in. Having irrelevant features in your data can decrease the accuracy of the models and make your model learn based on irrelevant features.

___How to select features and what are Benefits of performing feature selection before modeling your data?___

* __Reduces Overfitting:__ Less redundant data means less opportunity to make decisions based on noise.
* __Improves Accuracy:__ Less misleading data means modeling accuracy improves.
* __Reduces Training Time:__ fewer data points reduce algorithm complexity and algorithms train faster.

___Why don’t we give all the features to the ML algorithm and let it decide which feature is important?___
So there are three reasons why we don’t:

1. ___Curse of dimensionality — Overfitting:___

If we have more columns in the data than the number of rows, we will be able to fit our training data perfectly, but that won’t generalize to the new samples. And thus we learn absolutely nothing.

2. ___Occam’s Razor:___

We want our models to be simple and explainable. We lose explainability when we have a lot of features.

3. ___Garbage In Garbage out:___

Most of the times, we will have many non-informative features. For Example, Name or ID variables. Poor-quality input will produce Poor-Quality output.

Fortunately, Scikit-learn has made it pretty much easy for us to make the feature selection. There are a lot of ways in which we can think of feature selection, but most feature selection methods can be divided into three major buckets:

* ___Filter based:___ We specify some metric and based on that filter features. An example of such a metric could be correlation/chi-square.
* ___Wrapper-based:___ Wrapper methods consider the selection of a set of features as a search problem. Example: Recursive Feature Elimination.
* ___Embedded:___ Embedded methods use algorithms that have built-in feature selection methods. For instance, Lasso and RF have their own feature selection methods.

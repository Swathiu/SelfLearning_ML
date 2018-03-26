Knn is a basic, simple algorithm but yet very useful means used in discrete classification of data. It is based on supervised learning.
Every time a label has to be predicted for query point, it has to calculate the distance metric from the query point to all the data points
in the training set. Hence, it is computationally intensive and dependant on memory heavily. Hence, not very much suitable for large data 
sets. Given a number of neighbors, i.e k value, the algorithm predicts the label of the query point as the label which is repeated most 
amongst it's neighbors. So, it uses majority vote concept. Website (https://kevinzakka.github.io/2016/07/13/k-nearest-neighbor/) 
defines Knn as  - 

Given a positive integer K, an unseen observation x and a similarity metric d, KNN classifier performs the following two steps:
1. It runs through the whole dataset computing d between x and each training observation. 
    Let the K points in the training data that are closest to x be set A. (K is usually odd to prevent tie situations)
2. It then estimates the conditional probability for each class, that is, the fraction of points in A with that given class label.
   (Note I(x) is the indicator function which evaluates to 1 when the argument x is true and 0 otherwise)

                                P(y=j|X=x)=1K∑i∈AI(y(i)=j)
                                
Finally, our input x gets assigned to the class with the largest probability.

Data Set used for implementing Knn algorithm - IrisDataSet (https://archive.ics.uci.edu/ml/datasets/Iris)

There are two implementations here -
1. One of them is using Scikit learn
2. And the Other is the custom implementation of Knn Algorithm.

I have referred the website - https://kevinzakka.github.io/2016/07/13/k-nearest-neighbor/ for my understanding and clarity of Knn algorithm.

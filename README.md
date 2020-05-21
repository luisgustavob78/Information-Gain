# Information-Gain

# Introduction

Information Gain is a technique of data science to calculate the level of influence of the predictors variables in the output of the predicted variable in a classification machine learning problem using the concept of data entropy. This metric is a way to measure something like a "predictive power" of an attribute. To get to know it, let's see the definitions.

# Definitions

Entropy is a measure of how the target classes are distributed in a dataset. Using a binary 0 or 1 problem as an example, if 50% data are 0 and 50% are 1, we have entropy = 1 (total chaos). Mathematically:

    * entropy = -p0.log(p0) -p1.log(p1)
    
where p0 and p1 are the percentage of 0 and 1 class, respectivelly.

Information Gain is the numerical impact of an attribute in entropy of the dataset. Considering a categorical variable with A and B values, we can define mathematicallly the information gain of that variable like is following:

    * I.G. = entropy- [pA.(-p0A.log(p0A) -p1A.log(p1A)) + pB.(-p0B.log(p0B) -p1B.log(p1B))]
    
 # Algorithm
 
 First, we need to calculate the entropy of our dataset
 ![](https://github.com/luisgustavob78/Information-Gain/blob/master/data_entropy.png)
 
 Then, we get the information gain of each one of our variables
 ![](https://github.com/luisgustavob78/Information-Gain/blob/master/code_ig.png)
 
 The bigger is the information gain of a variable, the bigger is your predictive power.
 ![](https://github.com/luisgustavob78/Information-Gain/blob/master/reults_ig.png)

# Refereces

This content was extracted from the book "data science for business"



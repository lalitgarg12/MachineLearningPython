# MachineLearningWithPython
![image.png](image/machine_learning.png)<br><br>
Machine Learning is a latest __buzzword__ floating around. It desrves to, as it is one of the most interesting subfield of Computer Science.<br>
__What does Machine Learning really means?__<br>
Machine Learning is an application of artificial intelligence(AI) that provides systems the ability  to automatically learn and improve from experience without being explicitly programmed.<br>
__Machine Learning focuses on the development of computer programs__ that can access data and use it to learn for themsleves.<br>
The process of learning begins with data, such as, direct experience, or instruction, in order to look for patterns in data and make better decisions in the future based on the examples that we provide. __The primary aim is to allow the computers learn automatically__ without human intervention or assistance and adjust actions accordingly.
![image.png](image/mlflow.png)<br><br>

## Repository Overview
This repository is about different Machine Learning algorithm approaches as per the industry practices.

## Table of Contents
- [Profit Prediction](#section1)<br>
- [Classification - Logistic Reg](#section2)<br>
- [SVM Classification](#section3)<br>
- [Spam Detection](#section4)<br>
- [K-Means Clustering](#section5)<br>

___
<a id=section1></a>
### [Profit Prediction](./Profit%20Prediction)
![image.png](image/Profit%20prediction.png)
- You are the CEO of restaurant Franchise and are considering different cities for opening new outlet.
- The chain already has trucks in various cities and you have data for profits and population from the cities.
- You would like to use this data to help you select which city to expand to next.
- The dataset contains in the data folder of this Project.
- [Link for the Jupyter notebook](./Profit%20Prediction/Profit_Prediction.ipynb)
___
<a id=section2></a>
### [Probability of admission](./Classification-Logistic%20Reg)
![image.png](image/Chances-of-admission.png)
- You are the administrator of a university department and you want to determine each applicant's chance of admission based on their
results on two exams.
- You have historical data from previous applicants that you can use as a training set for logistic regression.
- For each training example, you have the applicant's scores on two exams and the admissions decision.
- [Link for the Jupyter notebook](./Classification-Logistic%20Reg/Prob_of_admission.ipynb)
___
### [Accepting or Rejecting Microchips based on test results](./Classification-Logistic%20Reg)
![image.jpg](image/microchip-test.jpg)
- Suppose you are the product manager of the factory and you have the test results for some microchips on two different tests.
- From these two tests, you would like to determine whether the microchips should be accepted or rejected.
- To help you make the decision, you have a dataset of test results on past microchips, from which you can build a logistic regression model.
- [Link for the Jupyter notebook](./Classification-Logistic%20Reg/Microchip_test.ipynb)

___
<a id=section3></a>
### [SVM Classification](./SVM-Classification)
![image.png](image/svm.png)
- We will see different examples of how SVM works.
- On 2D Dataset, with different values of C and Sigma usign Gaussian Kernels.
- On Trained dataset using learning best parameters from the function and cross validation.
- Visualizing linear and non-linear decision boundaries by SVM Classification.
- [Link for the Jupyter notebook](./SVM-Classification/SVM.ipynb)

___
<a id=section4></a>
### [Spam Detection](./Spam-Detection)
![image.png](image/spamintro.png)
## Basic Approach
When we choose to approach spam filtering from a machine learning perspective, we view the problem as a classification problem. That is, we aim to classify an email as spam or not spam (ham) depending on its features. In our case, the features are the count of each word in the email. 

## Pre Processing
After preliminary pre-processing (removing HTML tags and headers from the email in the data set), we take the following steps:
1. __Tokenize__ - We create "tokens" from each word in the email by removing punctuation.
2. __Remove meaningless words__ -  The text in red squares are stop-words, which should be removed. Stop-words do not provide meaningful information to the classifier, and they increase dimensionality of feature matrix. In addition to many stop-words, we removed words over 12 characters and words less than three characters.
3. __Stem__ -  The text in blue circle is converted to its "stem". Similar words are converted to its stem in order to form a better feature matrix. This allows words with similar meanings to be treated the same. For example, history, histories, historic will be considered same word in the feature matrix. Each stem is placed into our "bag of words", which is just a list of every stem used in the dataset. 
4. __Create feature matrix__ - After creating the "bag of words" from all of the stems, we create a feature matrix. The feature matrix is created such that the entry in row i and column j is the number of times that token j occurs in email i. 
- [Link for the Jupyter notebook](./Spam-Detection/Spam-Detection.ipynb)

___
<a id=section5></a>
### [K-Means Clustering](./KmeansCluster)
## Introduction

Who is your Customer? Sometime it is not very obvious or short to answer this. There are lots of ways to classify customers and divided them by groups. But since we have data, let's use data approach to answer this question.<br><br>
When you have data -- like a list of customers and what they bought -- and you need to create groups with similar characterestics using this data, we need a clustering approach.<br>
![image.png](image/clustering.png)
- __Clustering__ is part of the unsupervised machine learning techniques.
- It is unsupervised as the machine has no previous information about how it should group the entities.
- They try to create clusters with similar entities by analysing how close they are one from another.
- [Link for the Jupyter notebook](./KmeansCluster/kmeans.ipynb)

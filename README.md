# Pitch Prediction using Scikit-Learn
This is a fun pitch prediction model built with Scikit-Learn's Decision Tree Classification algorithm in Python. This model demonstrates the power of a simple machine learning model to make deterministic predictions using a large volume of training and testing data. 


This repo demonstrates and documents the use of Scikit-Learn's Decision Tree Classification Algorithm for use in predicting the next pitch in a major league baseball game. The sample data was provided to me with some level of encoding to obfuscate team names, player names, etc, and came by way of an interview process with a company intimately involved in designing sports books for sports betting. 

This model acts as scaffolding for other Decision Tree Classification projects for developers who may have little or no experience with Decision Tree Classification, particularly in Python. This model walks through accuracy/precision and error testing methods to help tune a model and improve estimation as a result. Note that this model was originally run with a maximum depth of 16 due to performance limitations reached in a Jupyter Notebook deployed on a computer with a 9th Generation Intel I7 processor and 32gb of RAM running at 2666 mhz. A future version of this may be designed on Azure Databricks to remove limitations on an an initial run to better optimize the Decision Tree Classification Model. Note that the documentation in this model supports a model depth that does not exceed 16, but the model could improve with a greater depth and is not likely to improve with a depth of less than 16. 

With the above in mind, the code in this template applies a great framework for self-taught data scientists to familiarize themselves with a number of features available in Scikit-Learn's Decision Tree Classification algorithm. 

The framework demonstrates:
1. Methods for exploring a sample of data used to make a prediction with visualizations that include histograms (evaluating the frequency of events) and scatterplots. 
2. Options for removing data elements that may cause errors in modeling (ie, removal of attributes that are null/have no data). 
3. Code for partitioning of data into training and test sets. 
4. Code for fitting a model to determine its state of overall accuracy/precision. 
5. Methods for error testing and tuning a Decision Tree Classification model. 
6. Comparisons of an initial model with no tuning vs. a tuned model. 
7. Partial methods for deploying a model like this for production in a commercial-cloud environment. 

This repository includes all files used for deploying building and analyzing the model. 

***A note of caution, running this model on a cloud platform with Databricks or another virtual environment that allows the execution of python code could result in charges that are in excess of hundreds or thousands of dollars. This is because of the large memory and compute requirements at runtime, which are necessary to iterate enough decision trees to identify an optimal tree depth and an optimal cost complexity alpha value for the model (if an end user chooses to deploy a model without a maximum depth). The model in its current form could lead to a large bill from a cloud provider depending upon which cloud compute and memory resources are defined for a model. The end user is responsible for any and all costs incurred by deploying this code on their own platform(s). ***

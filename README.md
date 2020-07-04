# Udacity ML Engineer Nanodegree Capstone --- Stock Price Prediction

This repository contains code and associated files for deploying ML models using AWS SageMaker.

### Inspiration

In the course Machine Learning Case studies, I learned how to use DeepAR to predict power usage. I would like to apply this technique to the finance world. Stock price data are also time series and can be analyzed using similar methods.

### Purpose

Using Neural Network to predict daily stock price values. More specifically, we will train the model using data of 2014, 2015, 2016 and use the trained model to predict close price (represented by rate of change) in 2017.

### Datasets and Inputs

Apple stock price data from 2013 to 2018 (Apple 2013-2018.csv). Inputs will be the rate of change (ROC) of close price.

### Project Design

* Loading and exploring the data
* Creating training and test sets of time series
* Formatting data as JSON files and uploading to S3
* Instantiating and training a DeepAR estimator
* Deploying a model and creating a predictor
* Evaluating the predictor


---

## Setup Instructions

The notebook Stock_Price_Prediction.ipynb provided in this repository are intended to be executed using Amazon's SageMaker platform. The following is a brief set of instructions on setting up a managed notebook instance using SageMaker, from which the notebooks can be completed and run.

### Log in to the AWS console and create a notebook instance

Log in to the [AWS console](https://console.aws.amazon.com) and go to the SageMaker dashboard. Click on 'Create notebook instance'.
* The notebook name can be anything and using ml.t2.medium is a good idea as it is covered under the free tier. 
* For the role, creating a new role works fine. Using the default options is also okay. 
* It's important to note that you need the notebook instance to have access to S3 resources, which it does by default. In particular, any S3 bucket or object, with “sagemaker" in the name, is available to the notebook.
* Use the option to **git clone** the project repository into the notebook instance by pasting `https://github.com/udacity/ML_SageMaker_Studies.git`

### Open and run the notebook of your choice

Now that the repository has been cloned into the notebook instance you may navigate to any of the notebooks that you wish to complete or execute and work with them. Additional instructions are contained in their respective notebooks.

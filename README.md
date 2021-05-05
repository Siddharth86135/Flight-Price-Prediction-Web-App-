# Flight Fare Prediction: 

## Table of Content
  * [Demo](#demo)
  * [Overview](#overview)
  * [Installation](#installation)
  * [Machine Learning Model Used](#machine-learning-model-used)
  * [Hyperparameter Tuning](#hyperparameter-tuning)
  * [Deployement on Heroku](#deployement-on-heroku)
  * [Directory Tree](#directory-tree)
 


## Demo
Link: [https://flight---fare---prediction.herokuapp.com/](https://flight---fare---prediction.herokuapp.com/)

[![](https://user-images.githubusercontent.com/51194972/95820933-a14d4680-0d46-11eb-99b8-de8e66944738.JPG)](https://flight---fare---prediction.herokuapp.com/)

## Overview
This is a Flask web app which predicts fare of Flight ticket.

## Installation
The Code is written in Python 3.6.10. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```
## Machine Learning Model Used

I used Random forest Machine Learning model in this project.

Random forest, like its name implies, consists of a large number of individual decision trees that operate as an ensemble. Each individual tree in the random forest spits out a class prediction and the class with the most votes becomes our model’s prediction

The fundamental concept behind random forest is a simple but powerful one — the wisdom of crowds. In data science speak, the reason that the random forest model works so well is:
A large number of relatively uncorrelated models (trees) operating as a committee will outperform any of the individual constituent models.


The low correlation between models is the key. Just like how investments with low correlations (like stocks and bonds) come together to form a portfolio that is greater than the sum of its parts, uncorrelated models can produce ensemble predictions that are more accurate than any of the individual predictions. The reason for this wonderful effect is that the trees protect each other from their individual errors (as long as they don’t constantly all err in the same direction).

## Hyperparameter Tuning

In this project I also used Hyperparameter tuning to fine tune the Random forest Regressor.

In machine learning, hyperparameter optimization or tuning is the problem of choosing a set of optimal hyperparameters for a learning algorithm. A hyperparameter is a parameter whose value is used to control the learning process. By contrast, the values of other parameters (typically node weights) are learned.

The same kind of machine learning model can require different constraints, weights or learning rates to generalize different data patterns. These measures are called hyperparameters, and have to be tuned so that the model can optimally solve the machine learning problem. Hyperparameter optimization finds a tuple of hyperparameters that yields an optimal model which minimizes a predefined loss function on given independent data. The objective function takes a tuple of hyperparameters and returns the associated loss. Cross-validation is often used to estimate this generalization performance.


## Deployement on Heroku
Login or signup in order to create virtual app. You can either connect your github profile or download ctl to manually deploy this project.

[![](https://i.imgur.com/dKmlpqX.png)](https://heroku.com)

Our next step would be to follow the instruction given on [Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python) to deploy a web app.

## Directory Tree 
```
├── static 
│   ├── css
├── template
│   ├── home.html
├── Procfile
├── README.md
├── app.py
├── flight_price.ipynb
├── flight_rf.pkl
├── requirements.txt
```

## Model Deployement

Taking ML models from conceptualization to production is typically complex and time-consuming. You have to manage large amounts of data to train the model, choose the best algorithm for training it, manage the compute capacity while training it, and then deploy the model into a production environment. Amazon SageMaker reduces this complexity by making it much easier to build and deploy ML models. After you choose the right algorithms and frameworks from the wide range of choices available, SageMaker manages all of the underlying infrastructure to train your model at petabyte scale, and deploy it to production.

1. Machine Learning Model Deployment Using Heroku Cloud

Heroku is a cloud Platform as a Service that helps developers quickly deploy, manage, and scale moderns applications without infrastructure headaches.f you want to deploy your model for the first time, I recommend that you try Heroku because it is flexible and easy to use.

It offers a wide range of services and tools to speed up your development and helps you avoid starting everything from scratch. It also supports several widely used programming languages like Python, Java, PHP, Node, Go, Ruby, Scala, and Clojure.

The good thing about Heroku is that it makes it easy to create, deploy and manage your app. You can do this right from the command line using the Heroku CLI (available for Windows, Linux, and Mac users).

On the deployment part, you can upload your trained machine learning model and source code onto Heroku by linking your Github repository to your Heroku account.


2. Machine Learning Model Deployment Using Microsoft Azure Functions

Azure Functions is a serverless cloud service provided by Microsoft Azure as a Functions-as-a-service (FaaS). Azure functions help developers offload infrastructure management tasks and focus on running their applications.

With serverless, you can write a snippet of code that runs your model and then deploy the code and machine learning model on Azure Functions and call it for prediction as an API. Azure functions are similar to Google cloud functions.

Azure Functions supports different functions developed in C#, F#, Node.js, Python, PHP, JavaScript, Java 8, Powershell Core, and TypeScript.

If you have a big machine learning model, then Azure functions is the right choice for you. It supports the deployment of large ML packages such as deep learning frameworks (Tensorflow and Pytorch).


3. Machine Learning Model Deployment Using AWS Lambda

AWS Lambda is a serverless computing service provided by Amazon as part of Amazon Web Services. AWS lambda helps you run your code without managing the underlying infrastructure.

With Lambda, you can upload your code in a container image or zip file. Lambda will automatically allocate computational power to run your code based on the incoming requests or events without requiring you to configure anything.

AWS Lambda allows your code to be associated with other AWS resources such as Amazon DyanamoDB table, Amazon S3 bucket, Amazon SNS notification, and Amazon Kinesis stream. Therefore you can easily deploy your machine learning model on AWS Lambda, and you can access it through an API using Amazon API Gateway. You can write Lambda functions in the following supported programming languages: Python, Java, Go, PowerShell, Node.js, Ruby, and C# code.

AWS Lambda is very cheap because you only pay when you invoke the lambda function (that is, when you make prediction requests). It can save lots of money compared to the cost of running containers or Virtual Machines. If you want to monitor the lambda functions you have created, AWS Lambda will do it on your behalf.

AWS Lambda will monitor real-time metrics including error rates, total requests, function-level concurrency usage, latency, and throttled requests through Amazon CloudWatch. Then you can view the statistics for each lambda function by using AWS Lambda Console or Amazon CloudWatch Console.

## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://flask.palletsprojects.com/en/1.1.x/_images/flask-logo.png" width=170>](https://flask.palletsprojects.com/en/1.1.x/) [<img target="_blank" src="https://number1.co.za/wp-content/uploads/2017/10/gunicorn_logo-300x85.png" width=280>](https://gunicorn.org) [<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/) 



Summary
---

Machine Learning Engineer on [Udacity](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009t).

Learn advanced machine learning techniques and algorithms and how to package and deploy your models to a production environment. Gain practical experience using Amazon SageMaker to deploy trained models to a web application and evaluate the performance of your models. A/B test models and learn how to update the models as you gather more data, an important skill in industry.

This program is intended for students who already have knowledge of machine learning algorithms.


Course Roadmap
---
---

* General Software Engineering Practices
* Object-Oriented Programing
* Web Development

A good data scientist should be able to write efficient code so their programs can work well in production.


Software Engineering Practices Pt1
---
* Write clean and modular code
* Improve code efficiency
* Add effective documentation
* Use version


Software Engineering Practices Part II
---
* Testing
* Logging
* Code reviews

Object Oriented Programming
---
* Object-oriented programming syntax

  * procedural vs object-oriented programming
  * classes, objects, methods and attributes
  * coding a class
  * magic methods
  * inheritance

* Using object-oriented programming to make a Python package

  * making a package
  * tour of scikit-learn source code
  * putting your package on PyPi

Introduction of Deployment and Cloud Computing
---

SagemMaker Key Features:

* Notebook Instances provide a convenient place to process and explore data in addition to making it very easy to interact with the rest of SageMaker's features.

* Training Jobs allow us to create model artifacts by fitting various machine learning models to data.

* Hyperparameter Tuning allow us to create multiple training jobs each with different hyperparameters in order to find the hyperparameters that work best for a given problem.

* Models are essentially a combination of model artifacts formed during a training job and an associated docker container (code) that is used to perform inference.

* Endpoint Configurations act as blueprints for endpoints. They describe what sort of resources should be used when an endpoint is constructed along with which models should be used and, if multiple models are to be used, how the incoming data should be split up among the various models.

* Endpoints are the actual HTTP URLs that are created by SageMaker and which have properties specified by their associated endpoint configurations. Have you shut down your endpoints?

* Batch Transform is the method by which you can perform inference on a whole bunch of data at once. In contrast, setting up an endpoint allows you to perform inference on small amounts of data by sending it do the endpoint bit by bit.

In addition to the features provided by SageMaker we used three other Amazon services.

In particular, we used **S3** as a central repository in which to store our data. This included test / training / validation data as well as model artifacts that we created during training.

We also looked at how we could combine a deployed SageMaker endpoint with **Lambda** and **API Gateway** to create our own simple web app.

Building model in SageMaker

- built-in algorithms
- Set the hyperparameters
- configure input data 

Deploying model in SageMaker
---
Key concepts:

- application (web app)
- endpoints
- api gateway
- lambda function
- model

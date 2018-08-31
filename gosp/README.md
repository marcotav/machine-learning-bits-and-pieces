## Churn Analysis [[view code]](http://nbviewer.jupyter.org/github/marcotav/machine-learning-classification-projects/blob/master/churn/notebooks/predicting-customer-churn.ipynb)
![image title](https://img.shields.io/badge/work-in%20progress-blue.svg) ![image title](https://img.shields.io/badge/statsmodels-v0.8.0-blue.svg) ![Image title](https://img.shields.io/badge/sklearn-0.19.1-orange.svg) ![Image title](https://img.shields.io/badge/seaborn-v0.8.1-yellow.svg) ![Image title](https://img.shields.io/badge/pandas-0.22.0-red.svg) ![Image title](https://img.shields.io/badge/numpy-1.14.2-green.svg) ![Image title](https://img.shields.io/badge/matplotlib-v2.1.2-orange.svg)

**The code is available [here](http://nbviewer.jupyter.org/github/marcotav/machine-learning-classification-projects/blob/master/churn/notebooks/predicting-customer-churn.ipynb) or by clicking on the.**

This project was done in collaboration with [Corey Girard](https://github.com/coreygirard/)

<br>

<p align="center">
  <img src="images/cellphone.jpg", width = "400">
</p>                                                                  
<p align="center">
  <a href="#goals"> Goals </a> •
  <a href="#importance"> Why this is important? </a> •
  <a href="#mods"> Importing modules and reading the data </a> •
  <a href="#dh"> Data Handling and Feature Engineering </a> •
  <a href="#Xy"> Features and target </a> •
  <a href="#pp"> Using `pandas-profiling` and rejecting variables with correlations above 0.9 </a> •
  <a href="#scale">  Scaling </a> •
  <a href="#mc">  Model Comparison </a> •
  <a href="#rf"> Building a random forest classifier using GridSearch to optimize hyperparameters </a>
</p>


<a id = 'goals'></a>
### Goals
From Wikipedia, 

> Churn rate is a measure of the number of individuals or items moving out of a collective group over a specific period. It is one of two primary factors that determine the steady-state level of customers a business will support [...] It is an important factor for any business with a subscriber-based service model, [such as] mobile telephone networks.

Our goal in this analysis was to predict the churn rate from a mobile phone company based on customer attributes including:
- Area code
- Call duration at different hours
- Charges
- Account length

See [this website](http://blog.yhat.com/posts/predicting-customer-churn-with-sklearn.html) for a similar analysis.

<a id = 'importance'></a>
### Why this is important? 

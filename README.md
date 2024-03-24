# classifier_comparison

# Introduction

In this application, the goal is to compare the performance of the classifiers, namely K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines. The dataset related to marketing bank products over the telephone is used for this application.

# Dataset

The dataset comes from the UCI Machine Learning repository [link](https://archive.ics.uci.edu/ml/datasets/bank+marketing) The data is from a Portugese banking institution and is a collection of the results of multiple marketing campaigns. We will make use of the article accompanying the dataset here for more information on the data and features.

**Exploratory data analysis:**

The dataset consists of 20 features alongside a target feature indicating whether the client subscribed a term deposit. There were lot of outliers observed in the initial analysis. 

| Input Variables |
|---|
| 1 - age (numeric) |
| 2 - job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown') |
| 3 - marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed) |
| 4 - education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown') |
| 5 - default: has credit in default? (categorical: 'no','yes','unknown') |
| 6 - housing: has housing loan? (categorical: 'no','yes','unknown') |
| 7 - loan: has personal loan? (categorical: 'no','yes','unknown') |
| 8 - contact: contact communication type (categorical: 'cellular','telephone') |
| 9 - month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec') |
| 10 - day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri') |
| 11 - duration: last contact duration, in seconds (numeric). |
| 12 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact) |
| 13 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted) |
| 14 - previous: number of contacts performed before this campaign and for this client (numeric) |
| 15 - poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success') |
| 16 - emp.var.rate: employment variation rate - quarterly indicator (numeric) |
| 17 - cons.price.idx: consumer price index - monthly indicator (numeric) |
| 18 - cons.conf.idx: consumer confidence index - monthly indicator (numeric) |
| 19 - euribor3m: euribor 3 month rate - daily indicator (numeric) |
| 20 - nr.employed: number of employees - quarterly indicator (numeric) |

| Output variable (desired target): |
|---|
| 21 - y - has the client subscribed a term deposit? (binary: 'yes','no') |
|  |


**Data Visualization:**

![Cars by Type Cylinders](/images/carTypeCylinders.png)



# Models Evaluation and Comparison

To start with, a baseline model was created with the help of scikit learn's DummyClassifier. DummyClassifier was fit with the model and accuracy score was calculated.
In the classifier analysis, K-Nearest Neighbor Classifier, Decision Tree Classifier and Support Vector Classifier default models were evaluated and their accuracy scores were calculated. Decision Tree Classifier performed the best with the best training and testing accuracy scores. 

Below is a summary table presenting the results of the different ML regressor models:

|          Model | Fit Time | train_acc | test_acc |
|---------------:|---------:|----------:|----------|
| KNN Classifier | 0.059760 |  0.885540 | 0.883143 |
| DTC Classifier | 0.224090 |  0.891194 | 0.884600 |
| SVC Classifier | 9.746953 |  0.887239 | 0.887594 |

To further improve the model, hyperparameter tuning was employed using gridsearchcv for Decision Tree Classifier and Support Vector Classifier and the accuracy scores were calculated. The scores 


# Summary of Findings



# Notebook

[Classifier Comparison](/prompt_II.ipynb)

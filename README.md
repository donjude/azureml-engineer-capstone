*NOTE:* This file is a template that you can use to create the README for your project. The *TODO* comments below will highlight the information you should be sure to include.

# Predicting the Probability of Mortality Caused by Heart Failure

*TODO:* Write a short introduction to your project.

This project is the final capstone project as part of Microsoft's sponsored Udacity Nanodegree programme [Machine Learning Engineer for Microsoft Azure](https://www.udacity.com/course/machine-learning-engineer-for-microsoft-azure-nanodegree--nd00333).

In this project I used an external dataset outside the Microsoft Azure environment to develop two Machine Learning models using `Azure AutoML` and `Logistic Regression model + Hyper Drive`.

Hyper Drive is a model optimization tool which was used to optimized the logistic regression model. The `AutoML` model and the `Logistic Regression + Hyper Drive` models were compared and the best performing model was chosen and deployed as a webservice REST API using Azure Container Instance (ACI). The REST API endpoint is then consumed using a Python HTTP request calls to produce scoring results.

## Project Workflow diagram

![workflow diagram](images/capstone-diagram.png)

*TODO: State which model performed better, giving the model name and the metrics for comparison

## Project Set Up and Installation

*OPTIONAL:* If your project has any special installation steps, this is where you should put it. To turn this project into a professional portfolio project, you are encouraged to explain how to set up this project in AzureML.

This section describe how the project can be setup to run on Azure Machine Learning service in the cloud.

1. Azure Subscription
In order to use or create an instance of Azure ML Workspace, you need to have an azure subscription which would provide you access to Microsoft Azure resources. You can [create a new subscription](https://azure.microsoft.com/en-us/free/) or access an existing suscription if you have.

2. Azure ML SDK and other library installation

## Dataset

### Overview
*TODO*: Explain about the data you are using and where you got it from.

The dataset [Heart failure clinical records](https://archive.ics.uci.edu/ml/machine-learning-databases/00519/heart_failure_clinical_records_dataset.csv), used in the development of the machine learning models, comes from the **University of California, Irvin (UCI)** [Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records#).

The dataset contains 299 observations and 12 clinical features with one binary target variable `death event`. This data was collected from patients who had heart failures, during their clinical follow-up period.

The same dataset can also be found on the [Kaggle site](https://www.kaggle.com/andrewmvd/heart-failure-clinical-data?select=heart_failure_clinical_records_dataset.csv) and according to the site description about the data, it states that:
> Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worlwide.
Heart failure is a common event caused by CVDs and this dataset contains 12 features that can be used to predict mortality by heart failure.

Below is a description of the dataset:

### Attribute Information

Thirteen (12) clinical features:

- age: age of the patient (years)
- anaemia: decrease of red blood cells or hemoglobin (boolean)
- high blood pressure: if the patient has hypertension (boolean)
- creatinine phosphokinase (CPK): level of the CPK enzyme in the blood (mcg/L)
- diabetes: if the patient has diabetes (boolean)
- ejection fraction: percentage of blood leaving the heart at each contraction (percentage)
- platelets: platelets in the blood (kiloplatelets/mL)
- sex: woman or man (binary)
- serum creatinine: level of serum creatinine in the blood (mg/dL)
- serum sodium: level of serum sodium in the blood (mEq/L)
- smoking: if the patient smokes or not (boolean)
- time: follow-up period (days)

Target variable:

- [target] death event: if the patient deceased during the follow-up period (boolean)

### Task
*TODO*: Explain the task you are going to be solving with this dataset and the features you will be using for it.

In this project I seek to predict the mortality (death event) caused by Heart failure using serveral supervised machine learning techniques to predict the binary class for the target/label `death event`. The dataset contains individual clinical information of patients as described in the data attributes above. All the features in the dataset would be used in this project.

### Access
*TODO*: Explain how you are accessing the data in your workspace.

To access the dataset from my Azure Machine Learning workspace, I first downloaded the dataset from the UCI repository and registered the dataset in my Azure ML workspace.

## Automated ML
*TODO*: Give an overview of the `automl` settings and configuration you used for this experiment

### Results
*TODO*: What are the results you got with your automated ML model? What were the parameters of the model? How could you have improved it?

*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Hyperparameter Tuning
*TODO*: What kind of model did you choose for this experiment and why? Give an overview of the types of parameters and their ranges used for the hyperparameter search


### Results
*TODO*: What are the results you got with your model? What were the parameters of the model? How could you have improved it?

*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Model Deployment
*TODO*: Give an overview of the deployed model and instructions on how to query the endpoint with a sample input.

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:
- A working model
- Demo of the deployed  model
- Demo of a sample request sent to the endpoint and its response

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.

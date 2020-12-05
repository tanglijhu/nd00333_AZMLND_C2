# Project Title: Operationalizing Machine Learning Pipeline and Deployed Endpoint

The project's goal is to operationalize a machine learning pipeline with a deployed REST endpoint. 

The dataset used contains the bank marketing information including age, job, marital status, education, housing, loan, poutcome, etc. It is a classification problem where the goal is to predict whether the client will subscribe to a term deposit. After Azure Studio automated machine learning training, the best model was generated based on the criteria of "accuracy". The best model was deployed as the endpoint, which serves out predictions about whether a client's tendency to subscribe to a term deposit. 

## Architectural Diagram

Step 1: bank marketing dataset registration;
Step 2: automated machine training as a classification problem with a creteria of "accuracy";
Step 3: best model generation "VotingEnsemble";
Step 4: REST endpoint deployment;
Step 5: prediction testing with the provided "endpoint.py" file. 

## Key Steps

### Step 1: bank marketing dataset registration

registered dataset:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/registered%20datasets.PNG?raw=true)

### Step 2: automated machine training as a classification problem with a creteria of "accuracy"

completed automated machine learning: 
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/auto-ml-completed.PNG?raw=true)

### Step 3: best model generation "VotingEnsemble"

best model:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/best%20model%20-%201.PNG?raw=true)

### Step 4: REST endpoint deployment:

"Application Insights" enabled: 
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/endpoint-after-running-log-file.PNG?raw=true)

running "logs.py":
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/running-logs-file.PNG?raw=true)

running swagger on localhost showing the HTTP API methods and responses from the model:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/swagger-running.PNG?raw=true)

### Step 5: prediction testing with the provided "endpoint.py" file

running "endpoint.py" against the API producing JSON output from the model:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/running-endpoint.PNG?raw=true)

### Step 6: create, publish, and consume a pipeline using the provided Jupyter Notebook 

created pipeline:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/pipeline-created.PNG?raw=true)

pipeline endpoint:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/pipeline-endpoint.PNG?raw=true)

"Use RunDetails Widget" in Jupyter Notebook:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/RunDetails-Widget-1.PNG)
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/RunDetails-Widget-2.PNG)

scheduled run:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/scheduled-run-pipeline-rest-endpoint.PNG)

## Screen Recording

Below is the link to a screen recording of the project in action: 
https://youtu.be/eWd3JfqJwyA

The screencast demonstrates:
1) a working deployed ML model endpoint;
2) the deployed endpoint;
3) the best AutoML model;
4) successful API requests to the endpoint with a JSON payload. 

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
N/A

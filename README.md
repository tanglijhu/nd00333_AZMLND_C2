# Project Title: Operationalizing Machine Learning Pipeline and Deployed Endpoint

The project's goal is to operationalize a machine learning pipeline with a deployed REST endpoint. 

The dataset used contains the bank marketing information including age, job, marital status, education, housing, loan, poutcome, etc. It is a classification problem where the goal is to predict whether the client will subscribe to a term deposit. After Azure Studio automated machine learning training, the best model was generated based on the criteria of "accuracy". The best model was deployed as the endpoint, which serves out predictions about whether a client's tendency to subscribe to a term deposit. 

## Architectural Diagram

For the real-time endpoint: 
With the registered bank marketing dataset, a classification automated machine learning training was performed with a criteria of "accuracy". 
After training, the best model was generated as of "VotingEnsemble" and was deployed as a real-time endpoint. 
The prediction was made by running the provided "endpoint.py" file. 

For the pipeline endpoint: 
The same registered bank marketing dataset was used. The automated machine learning training was performed with the use of a Jupyter Notebook. The primary metric used was "AUC_weighted". 
Afterwards, the pipeline with AutoMLStep was created. During the training, the AutoMLStep could be visualized with the use of "RunDetails" widget. 
The best model was retrieved and tested. 
The pipeline was publishd and the REST endpoint was generated to use for predictions. 

## Screen Shots

![registered dataset](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/registered%20datasets.PNG?raw=true)

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
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/RunDetails-Widget-1.PNG?raw=true)
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/RunDetails-Widget-2.PNG?raw=true)

scheduled run:
![alt text](https://github.com/tanglijhu/nd00333_AZMLND_C2/blob/tanglijhu-patch-2/scheduled-run-pipeline-rest-endpoint.PNG?raw=true)

## Screen Recording

Below is the link to a [screen recording](https://youtu.be/eWd3JfqJwyA) of the project in action: 

The screencast demonstrates:
1) a working deployed ML model endpoint;
2) the deployed endpoint;
3) the best AutoML model;
4) successful API requests to the endpoint with a JSON payload. 

## Suggestions to Improve



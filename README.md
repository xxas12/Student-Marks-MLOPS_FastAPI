# Student-Marks-MLOPS_FastAPI

## Description of the project files
This project include 4 files in total, 3 notebook files and 1 csv file those file are :
* data cleaning.ipynd
* model building.ipynd
* api.ipynd
* student marks.csv

## Data Analysis:
After doing some analysis we have found out that their is no need of data cleannig becuase there are no missing value in the provided data set, later on we found out there is huge corelation between the Marks column and time column and there not so much outlier in the given data.There is no need of feature engineering or any type of encoding. 
Check: data_Cleaning.ipynd

## Model Building
For building our model we used  linear regression the feature's used for our are the following columns from the "student marks.csv" file which are "number_courses" and "time_study" for prediction we use the "marks" column becuae we are trying to predict marks of the student on the basis of number of courses and study time, we used pickle for saving and loading the model. 
Check: model_building.ipynd

## Model Evaluation
Model accuracy on testing data set is 3.079 and R² is 0.94 whereas for training data Model Accuracy is 3.051 and R² is 0.93.
Check: model_building.ipynd

## MLOPS
For MLOPS we have used FastAPI with ngrok for secure end to end point for mlops for now only which takes two input float and int if the marks are not below 50 'you pass' message will be output otherwise 'you shall not pass'. 
Check: api.ipynd

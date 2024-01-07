# Prediction of heart disease using different Machine Learning Methods


![heart](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/2a305b47-666b-416d-9281-377ba7f063ff)

Cardiovascular disease (CVD) is any disease involving the heart or blood vessels.
Cardiovascular diseases are the leading cause of death worldwide except Africa. Together CVD resulted in 17.9 million deaths (32.1%) in 2015, up from 12.3 million (25.8%) in 1990.
Deaths, at a given age, from CVD are more common and have been increasing in much of the developing world, while rates have declined in most of the developed world since the 1970s




## Project Overview
In pursuit of find a reliable method to determine when a person could have heart disease 
a dataset with various parameters related to heart health was downloaded and several methods of 
Machine Learning were applied to it, in order to determine their reliability, the accuracy of each one was computed.

## Skills used in this project
* Data visualization using Python
* Logistic Regression
* Naive-Bayes method
* K-Neighbors classifier
* Decission Tree Regression
* Confusion Matrixes
* Accuracy Calculation


## Understanding the data
The dataset contains multiple columns with information about the patients


* Age : Age of the patient [years]
* Sex : Sex of the patient[1,0]
* cp : Chest Pain type chest pain type
  * Value 1: typical angina
  * Value 2: atypical angina
  * Value 3: non-anginal pain
  * Value 4: asymptomatic
* trtbps : resting blood pressure [in mm Hg]
* chol : cholestoral fetched via BMI sensor [in mg/dl] 
* fbs : (fasting blood sugar > 120 mg/dl) [1 = true; 0 = false]
* rest_ecg : resting electrocardiographic results [values 0,1,2]
* thalach : maximum heart rate achieved 
* exang : exercise induced angina [1 = yes; 0 = no]
* oldpeak : ST depression induced by exercise relative to rest
* slope : the slope of the peak exercise ST segment
* ca: number of major vessels [0-3] colored by flourosopy
* thal : heart rate
    * Value 0: normal
    * Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
    * Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
* target : 0= less chance of heart attack 1= more chance of heart attack

## Data Exploratory Analysis

The relation between positive cases of heart disease and the age of each person shows 
a clear increase in the positive cases between the 40 and 60 years old, as shown in the ages graph 


![cases_by_age](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/7e755043-3f5b-4b78-91f0-d550fc680f04)

We can see this more clearly in the normal distribution graph


![normal_dist](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/e40d8295-eadb-4272-8434-0a4470078bd9)

Another correlation found according to the sex shows how the patients of group 1 are slightly more likely to develop heart disease.


![pos_sex](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/a6627ea8-a0e2-4d6e-9448-69d639ccb846)



Unfortunately this is biased.

Looking at the total number of patients, the group 1 is formed by way more patients than group 0 in fact more than double, so it´s logical that there will be more positive cases.
A more accurate approach is the ratio between the total of patients by group and the positive cases, finding that the group 0 is more likely to suffer a heart disease.


![Captura de pantalla 2024-01-05 173159](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/c3844b7f-e01c-4145-919b-e98350e93324)


All the other parameters are more complex tests but they are related about a good health, generally speaking, these are the most influential parameters.


![heatmap](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/0421be2c-61fd-4b6d-a731-1b3c5f60c03b)


## Model Evaluation

Four different models were used:
* Logistic Regression
* Naive-Bayes
* K-Nearest Neighbour
* Decission Tree Regression

All these methods were used in the dataset, splitting the data in a training set and a test set we were able to train all the four models 
and predict new values, allowing us to calculate the accuracy of each one, as well as their confussion matrix.


![Captura de pantalla 2024-01-07 131316](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/79dac82d-d238-4b63-941c-740c89fcc7c9)



The Decission Tree Regressor resulted to be the most accurate and thus the one chosen to predict new data.


## Generating data to test the model


Once we have decided on the model to be used we create a dataset for four different patients with distinct
parameters randomly chosen 


![Captura de pantalla 2024-01-07 133957](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/56fc8d76-f657-40e8-9592-a5fb896597dc)


And by applying the Decission Tree Regression method we can finally preddict the less or more chances to get a heart attack for each one


![Captura de pantalla 2024-01-07 134147](https://github.com/Hector658/Prediction-of-Heart-Disease-Using-ML-methods/assets/146046209/7b8f3ff3-adb0-4e38-a77c-4bb2ea7b76d4)


## Bibliography

* https://en.wikipedia.org/wiki/Cardiovascular_disease
* https://www.healthline.com/health/heart-disease/statistics
*  https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset
*  https://scikit-learn.org/stable/#










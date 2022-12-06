# Streets-Repair-Projects-Reduction-in-San-Diego
****


# Forecasting street repair projects completion times 

This is a final project for ADS506: (https://github.com/mycunguyen/Streets-Repair-Projects-Reduction-in-San-Diego)

#### -- Project Status: [Completed]

## Project Intro
-The City of San Diego is known as the “Finest City in America''. That phrase does not translate to the roadways in San Diego as a majority of the streets are undergoing or in need of serious repair, “ reports suggest that 44% percent of the city’s streets are in poor condition, ranking San Diego 8th in the US for having the worst roads” (Hamparyan, 2017).  Road repairs are a necessity in the City of San Diego but that does not mean they are convenient to its residents. Graham (2021) describes one such bad road in San Diego, Gold Coast Drive, has seen more than 200 complaints over the years to the City of San Diego requesting repavement(pp.1). Residents of this road also report thousands of dollars in vehicle repairs due to vast amounts of potholes. San Diego’s local government is finally starting to realize that the 3,000 miles of roads in the City are in dire need of repairs and taking steps to improve roadways. Establishing a new program called “Sexy Streets'' the City of San Diego will be repairing roads and streets that are in underserved communities. With the increase of plans for road repairs it will be important to ensure that the process is completed timely and in an efficient manner. To meet this goal the City of San Diego will need to conduct analysis of past street repair projects to better understand the completion times for the new “Sexy Streets'' program. 


### Team 3
* Michael Nguyen

* Vannesa Salazar


### Methods Used
* Data preprocessing
* Exploratory Data Analysis
* Data Visualization
* Predictive Modeling
* Forecasting Modeling
* Exponential Smoothing
* Accuracy evaluation


### Technologies
* R, Rstudio
* Libraries:‘readxl’, ‘creditmodel’, ‘zoo’, ‘fpp2’, ‘readr’, ‘dplyr’, and ‘tibble’.


## Project Description

-This paper presents the model selection for forecasting how long a road repair project will take by using road projects of the past. Seasonality and trend were investigated to determine their presence or absence and then controlled. The following models were utilized throughout the project : Naive, Seasonal Naive, ARIMA, Simple Exponential, Holt-Winter, Moving Average, and Linear. Performance of each model was verified with the use of the accuracy function in Rstudio where the root mean square errors were compared to determine the model of best fit. The variety of models presented do determine models of good fit and the ability to determine the expected duration of a road repair project. 
-Keywords : Naive, ARIMA, Accuracy, forecast, prediction, fit, overfitting, models, trend, seasonality. Exponential, Holt-Winter. 



## Needs of this project

- data exploration/descriptive statistics
- data preocessing/data cleaning
- statistical modeling
- techincal report/notebook
- presentation- Pitch deck

## Required R Libraries
* Basics
* Import the following Libraries:‘readxl’, ‘creditmodel’, ‘zoo’, ‘fpp2’, ‘readr’, ‘dplyr’, and ‘tibble’.


## Getting Started

1. Clone this repository using the raw data.
2. Add additional code or make changes and push new code into repo. Code should be ran prior to adding to the repository in order to ensure cohesiveness. 



## Data Pre-Processing
-The data contains 24,934 instances and 20 attributes. The data is relatively complete and ready for preprocessing; however the data set has multiple projects that start on the same date resulting in duplicates which would not be ideal for model and forecasting. These duplicates must be dealt with prior to modeling. Additionally, a clear number of days was not established through the data set so an additional column was added using the difference between end date and start date and named num_days for how long a project took. 

## Duplicate Values
- To combat the issue with duplicate dates it was determined that the values would be averaged with the following columns: ‘length’, ‘width’, ‘paving miles’ and newly created column number of days. The resulting data frame consists of 1751 instances and 5 attributes.


## Modeling & Evaluation
*Naive
*Seasonal Naive
*ARIMA
*Simple Exponential
*Holt-Winter
*Moving Average
*Linear

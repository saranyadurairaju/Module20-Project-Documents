# Agriculture and Forest Land Emission Analysis

**Submitted By:** Biresh | Praveeja | Ruma | Saranya </br>
_Date_: November, 24th, 2021\
_Data Analytics & Machine Learning Project_ : **Emission Analysis** <br/>

![image](https://user-images.githubusercontent.com/85472349/142740221-742d9738-eb24-4d67-91f6-fa612810d4f5.png)


Presentation: [Link to Google Slides Presentation](https://docs.google.com/presentation/d/1YAfvlpk0U3Oy9Srs9rTvzcp4tBlyMZlRyR9JFlisfMc/edit#slide=id.g10116574057_0_2)

Analysis dashboard:  [Link to Web Page](http://emission-tableau1.herokuapp.com/)


## Table of Contents
  * [Overview](#view)
  * [Analysis](#start)
  * [FlowChart](#flowchart)
  * [Database](#data)
  * [MachineLearning](#machinelearning)
    * [LinearRegression](#linearregression)
    * [ClassificationAlgorithms](#classificationalgorithms)
  * [Visualization](#viz)
  * [Technologies](#tech)
  * [Recommendations](#future)
  * [Summary](#result)

## <a name="view"></a>Overview
Global warming is one of the biggest problems we are facing now. Not only industrialized emission, agriculture and forest land emissions also play a big role in contributing to global warming by releasing greenhouse gases (GHG) such as CO2, CH4, N2O. After this analysis we will know more about agriculture and forestland emission.  

This project aims to deliver detailed view of each Country, Element, Items that are contributing to emission each Year. Also using the Machine Learning model, the data is anlayzed and categorized into zones. Our purpose is to Analyze the Emission data and to create a complete system from Cleaning to Modelling. 

## <a name="start"></a>Analysis

The Uncleaned Emission and Population data are moved in to two data frames .
Dropped the Unit column as it contains the  same data.
Normalized the data by changing the Year columns to rows using the “melt” statement.
The column names are changed in to standard form. 
Dropped the Years from 1961 to 1989 as it have very negligible informations.
All the null values are changed to zeros.
The cleaned data is saved as CSV file and saved in AWS’ s3 bucket too.


The project consists of these portions:
```
PROJECT
├── .gitignore
├── README.md
├── config
│   ├── data-params.json
│   ├── env.json
│   ├── model.json
│   ├── process-params.json
│   ├── test-data-params.json
│   ├── test-model.json
│   └── test-process-params.json
├── imgs
├── notebooks
│   ├── prop_score.ipynb
│   └── sandbox.ipynb
├── references
│   └── .gitkeep
├── requirements.txt
├── run.py
├── index.html
├── index.md
└── src
│   ├── etl.py
│   ├── model_vod.py
│   ├── model.py
│   └── viz.py
```

## <a name="flowchart"></a>Flow Chart

## <a name="data"></a>Data Base

## <a name="machinelearning"></a>Machine Learning

#### <a name="linearregression"></a>Linear Regression
Linear graph 

#### <a name="classificationalgorithms"></a>Classification Algorithms
Zone between 0 to 3. 


## <a name="viz"></a>Visualization
This emission analysis is deployed publicly on Heroku, click [here](http://emission-tableau1.herokuapp.com//) to check it out!
 
 
## <a name="tech">Technologies</a>
This project was created with:
* JavaScript
* HTML/CSS
* D3
* Flask
* Python 3.8
* Pandas
* Jupyter Notebook

## <a name="future"></a>Recommendations

## <a name="result"></a>Summary

Completed Emission Analysis Webpage: [Emission_Analysis_Web](http://emission-tableau1.herokuapp.com/)
Analysis results in the static page: https://saranyadurairaju.github.io/Module20-static-webpage/

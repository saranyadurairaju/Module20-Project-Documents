# Agriculture and Forest Land Emission Analysis

**Submitted By:** Biresh Kundu | Praveeja Sasidharan Suni | Ruma Talukder | Saranya Durairaju </br>
_Date_: November, 24th, 2021\
_Data Analytics & Machine Learning Project_ : **Emission Analysis** <br/>


Presentation: [Link to Google Slides Presentation](https://docs.google.com/presentation/d/1YAfvlpk0U3Oy9Srs9rTvzcp4tBlyMZlRyR9JFlisfMc/edit#slide=id.g10116574057_0_2)

Analysis dashboard:  [Link to Web Page](http://emission-tableau1.herokuapp.com/)


![image](https://github.com/bireshk/DataAnalyticsProject/blob/main/Image/The-Glasgow-Climate-Change-Summit039s-Global-Stakes.jpg)


## Table of Contents
  * [Overview](#view)
  * [Analysis](#start)
  * [FlowChart](#flowchart)
  * [Database](#data)
  * [Machine Learning](#machinelearning)
    * [Linear Regression](#linearregression)
    * [Classification Algorithms](#classificationalgorithms)
  * [Visualization](#viz)
    * [Static Webpage](#staticpage)
    * [Dashboard](#heroku)
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
├── Data
│   ├── Emission_data.csv
│   ├── Image_Sources.txt
│   ├── Population_data.csv
│   └── schema.sql
├── Image
│   └── All Images
├── Scripts
│   ├── Cleaning_Analysis
│       ├── ETL_Emission_Population.ipynb  
│       └── Pyplot_Emission_Population.ipynb
│   ├── ML
│       ├── ML_Emission_Classification_CH4.ipynb  
│       ├── ML_Emission_Classification_N2O.ipynb
│       ├── ML_Regression_Analysis_CH4.ipynb
│       ├── ML_Regression_Analysis_N2O.ipynb
│       └── ML_Regression_Analysis_World.ipynb
│   ├── Tables
│       ├── Data_Emission_Population_Merge.ipynb  
│       ├── Data_SqlAlchemy_query.ipynb
│       └── Data_Subtable_Creation.ipynb
│   ├── Webpage_Static
│       ├── Images
│       ├── index.html
│       └── style.css
│   ├── Webpage_Tableau
│       ├── Static
│           ├── images
│           └── css
│       ├── composer.json
│       ├── index.html
│       └── index.php
```

## <a name="flowchart"></a>Flow Chart

## <a name="data"></a>Data Base

## <a name="machinelearning"></a>Machine Learning

In Machine Learning, Methane (CH4) and Nitrous Oxide (N2O) emissions are analyzed as it contributes more on Agriculture and Forest land emissions. Below are the list items contribute in each gas. 

![image](https://user-images.githubusercontent.com/85472349/141954151-80dd5f92-6b6c-4240-a29c-9208c55a253b.png)

### <a name="linearregression"></a>Linear Regression

Linear regression attempts to model the relationship between two variables by fitting a linear equation to observe data. Using Linear regression the most contributing items of top 3 countries and the Whole world data are analyzed and this results will help in figuring the action needed items for those countries.

**Global Green House Gas Emission Analysis**

![image](https://user-images.githubusercontent.com/85472349/141962584-68e4989b-5cc5-4c49-9c5c-1b83b70c42d1.png)


### <a name="classificationalgorithms"></a>Classification Algorithms

* Machine learning methods that predict the future Emission depends on many factors like soil temperature, air moisture, Volumetric Water Content(VWC)
* Classification algorithms will help us identifying the Emission values into different Zones for each Elements
* Classifying the Target variable “Zones” into Binary Values is not possible as the data is Imbalanced
* Multiclass classification is the problem of classifying instances into one of three or more classes
* Data pre-processing and Categorizing Element, Item, Year, Population, Emission features


#### Logistic Regression Classifier

Logistic regression is a simple yet very effective classification algorithm. Multinomial logistic regression is an extension of logistic regression that adds native support for multi-class classification problems. Below are the Confusion Matrix:

![image](https://user-images.githubusercontent.com/85472349/142752292-5bb6374d-8092-4ce2-b47e-659e0e341740.png)

![image](https://user-images.githubusercontent.com/85472349/142752300-9a3d445b-9678-49d7-a916-b94c3f1249ff.png)


#### Random Forest Classifier

A random forest classifier works with data having discrete labels or better known as class. It reduces overfitting in decision trees and helps to improve the accuracy. It is also flexible to both classification and regression problems and works well with both categorical and continuous values.

![image](https://user-images.githubusercontent.com/85472349/142752314-547b3c5d-23c4-4c5e-8fff-af6b766cfa3b.png)

![image](https://user-images.githubusercontent.com/85472349/142752316-060719b4-76b9-4f71-953a-e24d8c1b7683.png)


### ML Results

![image](https://user-images.githubusercontent.com/85472349/141973384-fcd1b24f-42be-4f14-a5db-994ff5471916.png)

### ML Summary

The above results show that the Logistic Regression Algorithm classifies the Emission more accurately than Random Forest Classifier. Since our data is Skewed (Stratify was used) and Imbalanced which results in more number of items in specific categories. This might be the reason that our Logistic performed better than the Random Forest. Also, Logistic regression performs better when the number of noise variables is less than or equal to the number of explanatory variables. (Noise variables - Difficult or impossible to control; Explanatory Variable - manipulated in an experiment by a researcher). So. which model performs better completely depends on our Data set.


For more details about Machine Learning Model, please visit : [ML_Repo](https://github.com/saranyadurairaju/Module20-Final-Assignment)

## <a name="viz"></a>Visualization
Have to add points
 
### <a name="staticpage"></a>Static Webpage

Analysis results in the static page: https://saranyadurairaju.github.io/Module20-static-webpage/

### <a name="heroku"></a>Dashboard

Completed Emission Analysis Webpage: [Emission_Analysis_Web](http://emission-tableau1.herokuapp.com/)
 
## <a name="tech">Technologies</a>
This project was created with:
* JavaScript
* HTML/CSS
* D3
* Flask
* Python 3.8
* Pandas
* Jupyter Notebook

## <a name="future"></a>Sources
datalink
For image sources : https://github.com/bireshk/DataAnalyticsProject/blob/main/Data/Image_Sources.txt


## <a name="future"></a>Recommendations

## <a name="result"></a>Summary





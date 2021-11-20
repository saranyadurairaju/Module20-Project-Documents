# Agriculture and Forest Land Emission Analysis

**Submitted By:** Biresh | Praveeja | Ruma | Saranya </br>
_Date_: November, 24th, 2021\
_Data Analytics & Machine Learning Project_ : **Emission Analysis** <br/>

![image](https://user-images.githubusercontent.com/85472349/142740221-742d9738-eb24-4d67-91f6-fa612810d4f5.png)


Presentation: [Link to Google Slides Presentation](https://docs.google.com/presentation/d/1YAfvlpk0U3Oy9Srs9rTvzcp4tBlyMZlRyR9JFlisfMc/edit#slide=id.g10116574057_0_2)

Analysis dashboard:  [Link to Web Page](http://emission-tableau1.herokuapp.com/)


## Table of Contents
  * [Overview](#overview)
  * [Analysis](#analysis)
  * [FlowChart](#flowchart)
  * [Methods of Recommendation](#machine-learning)
    * [Similarity-Based CF](#similarity-based)
    * [User-Based CF](#ratings-based)
  * [Technologies](#technologies)

## <a name="overview"></a>Overview
Global warming is one of the biggest problems we are facing now. Not only industrialized emission, agriculture and forest land emissions also play a big role in contributing to global warming by releasing greenhouse gases (GHG) such as CO2, CH4, N2O. After this analysis we will know more about agriculture and forestland emission.  

This project aims to deliver detailed view of each Country, Element, Items that are contributing to emission each Year. Also using the Machine Learning model, the data is anlayzed and categorized into zones. Our purpose is to Analyze the Emission data and to create a complete system from Cleaning to Modelling. 

## <a name="analysis"></a>Analysis


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

## <a name="machine-learning"></a>Machine Learning

#### <a name="similarity-based"></a>Based on Similarity
This recommendation will be based on similarity between beers. Select one of the beers you like and a factor you think is the most important between flavor, aroma and texture for the beer. 

#### <a name="ratings-based"></a>Based on Ratings
This recommendation will be based on your ratings for three beers that you choose to rate. Select three beers you know and rate them - ratings can be between 1 to 5. 


## Deployment
This app is deployed publicly on Heroku, click [here](https://beer-recommendation-app.herokuapp.com/) to check it out!
 
 
## <a name="technologies">Technologies</a>
This project was created with:
* JavaScript
* HTML/CSS
* D3
* Flask
* Python 3.8
* Pandas
* Jupyter Notebook



Find the completed Toronto New Restaurant Analysis dashboard here: [Beer Recommendation App](https://beer-recommendation-app.herokuapp.com/)

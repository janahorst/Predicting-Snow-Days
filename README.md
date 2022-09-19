# Predicting-Snow-Days
In this repository, I predict if it will snow on a specific date with data from the public data set of google cloud via big query.

# Goal:
The goal of the analysis was to predict whether it would snow 13 years ago tomorrow. 

# Data:
The data comes from Google's public data set. The data includes weather information from various weather stations, such as snow, side, and temperature.

# Steps to get the data:
1. To prepare for the analysis, I created a project on Google Cloud, activated the BigQuery API and downloaded the credentials for this project as a Json file. Since this was my first time working with Google Cloud and the BigQuery API, downloading the credentials in particular was a hurdle at first. However, by googling I was able to solve this problem.
2. The second step was to connect BigQuery to my Jupiter notebook.
3. Once the connection between the BigQuery API and the notebook was established, I was able to prepare and download the data with SQL queries as described in the tasks.

# Analyse:
Since the analysis is about predicting whether it will snow (snow: yes/no) I decided to use a classification model and used XGBoost in the analysis. This allowed me to predict whether it will snow on the specific date at the different stations or not.
The XGBoost model correctly predicted the snow at the various stations without making a prediction error. Since a 100% correct model is very unlikely, there could be an error in the preparation of the data or in the analysis. 

# Further steps:
I will take a closer look at the accuracy problem when I have more time to develop the model.
- Preparations: I would  research further how to properly incorporate date variables into the XGBoost model and check the warning messages I got in the notebook.
- Model: If I had more time, I would also look closer at the feature importance and tune the model if necessary. 


# Udacity_AirBnb
A data science project on AirBnb data (Seattle and Boston)
My post on Medium : https://medium.com/@benny.vanhoof/boston-seattle-cf8f14100bd3
1) Project Motivation
***********************
The aim of the project was to define at least three questions for which the answers can be taken from an Airbnb dataset. Each question should be clearly defined and the answer to every question must be clearly motivated and documented with data science techniques.

2)Libraries
************
The following Python libraries should be loaded to run the code in the jupyter notebook:

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler,MinMaxScaler
from sklearn.ensemble import BaggingClassifier, RandomForestClassifier, AdaBoostClassifier
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import fbeta_score, accuracy_score
import geopandas as gpd
import folium

3) Files
********
The files are download from Kaggle : https://www.kaggle.com/airbnb/seattle
Two sets of three files are used: calendar.csv, listings.csv and reviews.csv. 
The calendar file contains information on a day by day base of a specific house was available for rent or not and at which price.
The listings file is a kind of catalog file that contains detailed information (92 different parameters) about each house. Each house is defined by an id and we find the same id's back in the calendar file.
The reviews file contains the same house id and contains the different reviews that were reported for each house. I will not use this information in this notebook.

4) Results
**********
The notebook shows a choroplet map with a geographic presentation of the rental prices in Boston and Seattle.
It shows also that the most predictive features for the price category are different in Seattle, compared to Boston.
The third part of the analysis is about the monthly and weekday spread of the rentals.

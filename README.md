# Airbnb Boston Price per Night Analysis

Machine Learning project aiming to predict pricing for Airbnbs in Boston based on location, size, and review scores.
The motivation for the project is to help new airbnb host list their properties at a competative price that will lead to a consistant bookings.

_________________________________________________________


### Installations

- import numpy as np
- import pandas as pd
- import matplotlib.pyplot as plt
- from sklearn.linear_model import LinearRegression
- from sklearn.model_selection import train_test_split
- from sklearn.metrics import r2_score, mean_squared_error
- import seaborn as sns

_________________________________________________________


### Files

#### calendar.csv
The calendar.csv file provided data consisting of listind_id, date, availability, and price. The file displayed the availabilty status of a listing. If availability was false then price would be $0. 

#### listings.csv
The listings.csv file provided the bulk ot the data.
It consisted of the data displayed when searching for an Airbnb to rent
Data such as:
  - Location
  - Host identification
  - Size and Spec of the property
  - Review scores of the property
  - Detailed descriptions of the Airbnb

#### reviews.csv
The reviews.csv file provided data about the reviewer and their comments about their stay at the Airbnb

_________________________________________________________


### Analysis

Results from a Linear Regression Model

#### Location
- Airbnbs are priced higher in zipcode 02116.
- Review score on location also increases the price
#### Size
- Host are more likely to charge more for renting the entire home but house tend to be cheaper
- Host renting out apartments will charge less
- A private room also tends to cost less.
- Airbnbs with 1-2 beds or one bathroom tend to be cheaper
- Airbnbs with 2 bedrooms or 2 bathrooms will cost more a night.
- Host charge more for real beds
- How many an airbnb can accommodate will increase the price
#### Reviews
- Host review ratings score and review location scores will have a positive influence on pricing
- Review score values and review score check-in has a negative influence on pricing
- Review score of cleanliness will raise the prices.


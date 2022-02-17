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
- Airbnbs in Jamaica Plains are lower in price unless it is cleansed then the price is higher.
- Neighborhoods with cheaper airbnb properties:
    - Allston-Brighton
    - Dorchester
    - zipcode 02130
    - South End
- Neighborhood with more expensive airbnb properties:
    - Beacon Hill
    - South Boston
    - Back Bay
    - zipcode 02116 
- Review score on location also leads to increased price

#### Size
- Renting a house will have a lower price while its the opposite for a condo and apartment.
- Renting the entire house or just a private room both increase the price
- Number of beds, bedrooms, and bathrooms will have an influence on pricing
    - 0-2 bedrooms lower the price
    - 1 bathroom has a negative effect on pricing
    - 2 bathrooms increase the pricing
    - 3 beds lower the price more than 1-2 beds
    - Real beds increase the price
- How many an airbnb can accommodate will increase the price

#### Reviews
- Host review ratings score and review location scores will have a positive influence on pricing
- Review score values and review score check-in has a negative influence on pricing
- Review score of cleanliness and communication will raise the prices. 


# MS-PHASE1-PROJECT

# Overview

This repo helps to determine the relationship between various aircraft and their associated risks, such as injuries and damages. The ultimate goal is to provide data-driven recommendations to the company regarding the purchase and operation of aircraft with the lowest potential risks, ensuring safer and more cost-effective operations.

# Business Problem

Your company is expanding in to new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating airplanes for commercial and private enterprises, but do not know anything about the potential risks of aircraft. You are charged with determining which aircraft are the lowest risk for the company to start this new business endeavor. You must then translate your findings into actionable insights that the head of the new aviation division can use to help decide which aircraft to purchase.

# The Data

The data we worked with were from datasetLinks to an external site: Kaggle ( https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses) from the National Transportation Safety Board that includes aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters.

# Questions to consider:

What are the aircraft types involved in aviation accidents? 

Is their a relation between the aircraft types or make and the total injuries?

What is the relation between the purpose of flight for the specific aircrafts and the injuries? 

What is the severity of Aviation accidents by Aircraft types?

# Sources of data 

1.AviationData to an external site (Kaggle)
2.USState_Codes to an external site(Kaggle)

# Description of data 

AviationData ~ The datatypes include float64(5), object(26), 88889 entries, 0 to 88888,Data columns (total 31 columns):
USState_Codes ~ The dataset include object(2), 62 entries, 0 to 61 Data columns (total 2 columns):

Numpy for high level mathematical functions and working with Arrays import numpy as np 
Pandas for data manipulation and analysis for tablular data,import pandas as pd 
Seaborn and matplotlib for data visualization import seaborn as sns import matplotlib.pyplot as plt %matplotlib inline

# Loading data

df1 = pd.read_csv('AviationData.csv',encoding='ISO-8859-1', low_memory=False) 
df2 = pd.read_csv('USState_Codes.csv', encoding='ISO-8859-1')

# Cleaning data 

Checking for the null values ~ (df1.isna().sum() / len(df1)) * 100 and dropping the null values 
Dropping the duplicates custom_fill_na(value): 
Filling the missing values with any value

# Visualizations 

![output](https://github.com/user-attachments/assets/4a8ca5af-4713-40e2-ae04-59bde218ba84)

![output 2](https://github.com/user-attachments/assets/1cbea1ef-d439-4697-9e92-3f97e1301a3b)

![output 3](https://github.com/user-attachments/assets/5b0fe1af-6eff-4650-b435-c6748864f867)



# Conclusions

Project will consider the dataset: 'AviationData_cleaned.csv' 
The bottom line for the company to determine on which aircraft to use will be inflenced by the number of injuries and the damages brought about by accidents as well as the make and model of the aircraft.
This will as well influence the type of purpose of flight the company chooses for their operations.

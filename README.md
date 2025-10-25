# The-impact-of-Tariffs-on-GDP-per-capita-Growth
What is the impact of tariffs on the U.S economy?
Tariffs have become a big economic discussion point, to really understand impacts of Tariffs on the economy I have analyzed the US GDP growth from 2000 to 2024. There are different metrics that have also been impacted by the use of tariffs through the years such as Unemployment, and Inflation rate. The relations between these metrics is important

# Libraries Used:

import pandas as pd   #Library for Data manipulation and Analysis

import numpy as np    #Library for Data manipulation

import matplotlib.pyplot as plt #Library for Data visualization

import seaborn as sns  #Library for data visualization

from sklearn import metrics #Library for Models score

from sklearn.model_selection import train_test_split #Splitting the data into training and test set

from sklearn.model_selection import train_test_split #Splitting the data into training and test set

from sklearn.tree import plot_tree  # plot the decision tree

from sklearn.model_selection import KFold, cross_val_score #Lets bring in the cross validation function to improve the score

import xgboost as xgb #lets import the xgboost model library

from xgboost import XGBClassifier #lets import the XGBclassifir

#Libraries to get different metric scores
from sklearn import metrics
from sklearn.metrics import (
    confusion_matrix,
    accuracy_score,
    precision_score,
    recall_score,
    f1_score,
)




# Libraries installed
%pip install sklearn  #Lets install Sklearn

%pip install Xgboost  #lets install Xgboost


# Data used on the Analysis
[US_Economy.csv](https://github.com/user-attachments/files/23139008/US_Economy.csv)

# Notebook used in the Analysis

http://localhost:8892/notebooks/Desktop/Udacity/Project%201/The%20impact%20of%20Tariffs%20on%20the%20US%20economy.ipynb

#  Summary of the results

The analysis examines the multifaceted impact of tariffs on the U.S. economy, particularly focusing on how they influence GDP per capita growth, the labor market, and the intricate relationship between inflation and economic expansion. It suggests that tariffs have an indirect influence on GDP per capita growth through their effects on inflation and unemployment. While the direct impact of tariffs on the labor market appears limited, they may indirectly affect it through unemployment rates. Furthermore, the analysis underscores the notable correlation between inflation and GDP per capita growth, with inflation playing a significant role in shaping consumer spending and, consequently, the overall economic landscape.

# Acknowledgements
 Data Credit: https://databank.worldbank.org/
 
 License: Anancoda Jupyter Notebook

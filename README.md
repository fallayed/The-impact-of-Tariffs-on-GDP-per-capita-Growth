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
Country Name,Country Code,Time,Time Code,"Inflation, consumer prices (annual %) [FP.CPI.TOTL.ZG]","Unemployment, total (% of total labor force) (national estimate) [SL.UEM.TOTL.NE.ZS]","Tariff rate, applied, weighted mean, all products (%) [TM.TAX.MRCH.WM.AR.ZS]","Labor force, total [SL.TLF.TOTL.IN]",GDP per capita growth (annual %) [NY.GDP.PCAP.KD.ZG]
United States,USA,2000,YR2000,3.37685727149929,3.992,2.1,147139887,2.92586254690673
United States,USA,2001,YR2001,2.82617111885407,4.731,2.11,148213470,-0.0387319301160716
United States,USA,2002,YR2002,1.58603162650601,5.783,2.16,149241895,0.761236857470422
United States,USA,2003,YR2003,2.27009497336115,5.989,1.96,149992325,1.91588247707845
United States,USA,2004,YR2004,2.67723669309172,5.529,1.79,151218126,2.89111091450374
United States,USA,2005,YR2005,3.3927468454955,5.084,1.75,153120588,2.53411070471215
United States,USA,2006,YR2006,3.22594410070404,4.623,1.7,155267046,1.79819874621896
United States,USA,2007,YR2007,2.85267248150138,4.622,1.55,156588966,1.03834382253567
United States,USA,2008,YR2008,3.839100296651,5.784,1.58,158272885,-0.828888121169271
United States,USA,2009,YR2009,-0.355546266299747,9.254,1.71,158353162,-3.42683194053784
United States,USA,2010,YR2010,1.6400434423899,9.633,1.66,158330168,1.82992369865936
United States,USA,2011,YR2011,3.156841568622,8.949,1.67,158537150,0.762796403185064
United States,USA,2012,YR2012,2.06933726526067,8.069,1.67,159682753,1.47570596859667
United States,USA,2013,YR2013,1.46483265562717,7.375,1.67,160132463,1.34816252728235
United States,USA,2014,YR2014,1.62222297740817,6.168,1.69,160876331,1.71094543865911
United States,USA,2015,YR2015,0.118627135552451,5.28,1.69,161927418,2.12741138238411
United States,USA,2016,YR2016,1.26158320570536,4.869,1.65,163886456,1.02266588951608
United States,USA,2017,YR2017,2.13011000365961,4.355,1.66,165597316,1.75014095244312
United States,USA,2018,YR2018,2.44258329692817,3.896,1.59,166999339,2.36444249959189
United States,USA,2019,YR2019,1.81221007526021,3.669,13.78,168920514,2.05676589936279
United States,USA,2020,YR2020,1.23358439630629,8.055,1.52,166565059,-2.56180738365786
United States,USA,2021,YR2021,4.69785886363742,5.349,1.47,167182196,5.8883410395074
United States,USA,2022,YR2022,8.00279982052121,3.65,1.49,169494100,1.92386172915427
United States,USA,2023,YR2023,4.11633838374488,3.638,..,172300802,2.03559987696194
United States,USA,2024,YR2024,2.94952520485207,4.022,..,174173594,1.79735044324696
,,,,,,,,
,,,,,,,,
,,,,,,,,
Data from database: World Development Indicators,,,,,,,,
Last Updated: 10/07/2025,,,,,,,,

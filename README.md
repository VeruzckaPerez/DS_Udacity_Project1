
# Forecast AirBnb prices in Seattle

## Motivation
When traveling it is important to find accommodation that fits the traveler's budget or for the traveler to know an approximate amount of how much it will cost to stay in a place with the characteristics of their preference.
For me it is important that the traveler knows if the price they are paying for a lodging is fair or above what is estimated.

## Libraries
### General
* import pandas as pd
* import numpy as np 
* import ast

### Plots
import matplotlib.pyplot as plt
import seaborn as sns

### ML
* import statsmodels.api as sm
* import statsmodels.formula.api as smf
* from statsmodels.stats.diagnostic import het_breuschpagan
* from statsmodels.stats.outliers_influence import variance_inflation_factor
* from statsmodels.tools.eval_measures import rmse
* from scipy import stats
* from sklearn.model_selection import train_test_split
* from typing import Union

## Files 
In the repository you will find 2 files:
* forecast_airbnb_prices.ipynb file: is the jupyter file that contains the code
* listings.csv: is the file that contains the data used in the forecast_airbnb_prices.ipynb file

## Summary of Results:
An Ordinary Least Squares model was used to predict prices in Seattle, however the results were not as expected, since the model is not representative enough. r2 of the model is: 0.601, that is, the model explains 60.7% of the data

It is recommended to use a more robust model to obtain best results

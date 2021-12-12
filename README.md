# Co2-Emissions

## Summary

this notebook describe the co2 emissions per regions and countries, that will help you calculate the Co2 emissions
and track the changes in Co2 emissions around the world, to read more about Co2 emissions and climate change please
read this article 
[Climate Change and solutions to save world] (https://medium.com/@mohamed_rabiem/climate-change-and-solutions-to-save-world-2156f8b61041)

## Installation 

 install jupyter notebook > python -m pip install jupyterlab📔 
 install pandas numpy, matplotlib pacages
 
 ''' 
 # Necessary imports
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sb
%matplotlib inline

# Read the regions, country meta data
countries = pd.read_csv('API_EN.ATM.CO2E.PC_DS2.csv')
countries_metadata = pd.read_csv('Metadata_Country.csv')
regions= pd.read_excel('Regions.xlsx',sheet_name='Sheet1')
regions.head()

 '''
 
## Deploy

upload the csv file and the ipynp file to jupyter notebook



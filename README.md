# Co2-Emissions

## Summary

this notebook describe the co2 emissions per regions and countries, that will help you calculate the Co2 emissions
and track the changes in Co2 emissions around the world, to read more about Co2 emissions and climate change please
read this article 
[Climate Change and solutions to save world] (https://medium.com/@mohamed_rabiem/climate-change-and-solutions-to-save-world-2156f8b61041)

![GettyImages-155141288-polar-bear-hero](https://user-images.githubusercontent.com/15274589/145721023-ddc8fb44-ee7e-4a14-a7db-bf6e60bea21c.jpg)


## Installation 

 install jupyter notebook > python -m pip install jupyterlab📔 
 install pandas numpy, matplotlib pacages
 
 
 ## Necessary imports
```import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sb
%matplotlib inline
```
 
## Deploy

upload the csv file and the ipynp file to jupyter notebook


## Get the Co2 emissions by Region for 2018
```
regionsIn2018 = regions.groupby('Region')[2018].mean().reset_index()
regins2018Ds = pd.DataFrame(regionsIn2018)
regins2018Ds.set_index('Region', inplace=True)
regins2018Ds

```
![ByRegion](https://user-images.githubusercontent.com/15274589/145727704-1127b585-9be6-4557-a88d-4ffc855465ac.PNG)

## Get the Co2 emissions reduction from 2008 to 2018

```
Co2EmissionsFor10Years = regions[['Region','2008','2009','2010','2011','2012','2013','2014','2015','2016','2017','2018']]
SumOfCo2PerYear=pd.DataFrame(Co2EmissionsFor10Years.sum())
SumOfCo2PerYear
![ClimateChange](https://user-images.githubusercontent.com/15274589/145732459-0edea0fe-a326-4ae7-91c5-baa5bceb471e.PNG)


```



## Get Countries with low Co2 emissions

```
CountriesCo22018.sort_values(by=["2018"], inplace = True)
CountriesCo22018.head(10)
```
![CountrieswithlowCo2emissions](https://user-images.githubusercontent.com/15274589/145721107-2ecf2a96-88b9-4146-9227-8d6b8cd633f9.PNG)

![Top 10 Countries](https://user-images.githubusercontent.com/15274589/145732374-88c7056a-2335-4977-a86e-b733c9652e10.PNG)


# Acknowledgment

### The data set provided from the internet from this website : https://data.world/search?context=community&q=ESG&type=all


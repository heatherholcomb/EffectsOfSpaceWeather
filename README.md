# EffectsOfSpaceWeather
## High Level Description
#### Space Weather describes the variations in the space environment between the sun and earth. In particular, Space Weather describes the phenomena that impact systems and technologies in orbit and on Earth. Space Weather can occur anywhere from the surface of the sun to the surface of the earth. I will also be doing a prediction model to see if we can predict Space Weather.  
## Space Weather Data
#### Space Weather Data was taken from: https://celestrak.com/
#### The Space Weather Data was cleaned ahead of time, meaning there was a header in the file used and it was faster to remove the header and load the data rather than attempt to remove the header through python. 
#### Data Time Frame: The space weather data contains data ranging from 1957-2020
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/SpaceWeatherTimeFrame.png" alt="Space Weather Time Frame" title="Space Weather Time Frame" />

#### Data Description: The Space Weather data used contains the following Columns: 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/SpaceWeatherColumns.png" alt="Space Weather Columns" title="Space Weather Columns" />

#### A description of these data fields can be found here: https://celestrak.com/SpaceData/SpaceWx-format.php
#### Note that the columns shown in the image have been renamed from the original dataset. 

## Climate
#### Climate Data was taken from: https://www.ncdc.noaa.gov/
#### Data Description: The climate data used for this project includes monthly climate data ranging from 01/01/2000 - 12/31/2019 and contains weather data from 5 different weather stations including:
#### -London Corbin Airport, KY
#### -Jerome CO Airport, ID
#### -Salina Municipal Airport, KS
#### -Greenville Main Forestry Service, ME
#### -Annapolis NAF, MD
#### The climate data used for this project contains the following columns: 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/ClimateColumns.png" alt="Climate Columns" title="Climate Columns" />

#### Note that the columns above still need to be identified and cleaned to make sense. 

## Final Climate and Space Weather Data
#### The Space Weather Data is a subset of the original data as shown below:
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/SpaceWeatherSubset.png" alt="Subset of Space Weather" title="Subset of Space Weather" />

#### The Climate Data is a subset of the original data as show below: 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/ClimateSubset.png" alt="Subset of Climate Data" title="Subset of Climate Data" />

#### Both the Space Weather Data and the Climate data were indexed by Year and Month and then merged as shown below: 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/MergedSpaceClimateData.png" alt="Merged Data" title="Merged Data" />

### Average Wind Speed from Merged Data
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/MergedDataGraph.png" alt="Merged Data" title="Merged Data" />

## Regression Models
#### Simple Linear Regression model - How does the Kp index affect Wind? 

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/SimpleLinearRegressionWindKp.png" alt="How does Kp Index affect wind" title="How does Kp index affect wind" />

#### Simple Linear Regression - How does Kp index affect Temperature? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/SimpleLinearRegressionTempKp.png" alt="How does Kp Index affect temperature" title="How does Kp index affect temperature" />

#### Multiple Linear Regression Model - How does the Kp Index, Solar Radio Flux, Flux Qualifier and F10_7 values affect Average Wind Speed? 

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/MultipleLinearRegression.png" alt="Multiple Regression" title="Multiple Regression" />

#### Multiple Linear Regression Model - How does the Kp Index, Solar Radio Flux, Flux Qualifier and F10_7 values affect Average Temperature? 

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/MultipleLinearRegression2.png" alt="Multiple Regression" title="Multiple Regression" />

#### Multiple Linear Regression Model - How does Kp Index, Solar Radio Flux, Flux Qualifier and F10_7 values affect Precipitation? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/MultipleLinearRegression3.png" alt="Multiple Regression" title="Multiple Regression" />

## Clustering 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/KMeans.png" alt="KMeans Clustering" title="KMeans Clustering" />

## Time Series

## Space Weather Predictions
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/SpaceWeatherPred.png" alt="Space Weather Prediction" title="Space Weather Prediction" />

## References: 

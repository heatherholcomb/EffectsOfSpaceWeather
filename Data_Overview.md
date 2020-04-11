# Data Description and Overview

### Space Weather Data
#### Space Weather Data was taken from: https://celestrak.com/
#### The Space Weather Data was cleaned ahead of time, meaning there was a header in the file used and it was faster to remove the header and load the data rather than attempt to remove the header through python. 
#### Data Time Frame: The space weather data contains data ranging from 1957-2020
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/SpaceWeatherTimeFrame.png" alt="Space Weather Time Frame" title="Space Weather Time Frame" />

#### Data Description: The Space Weather data used contains the following Columns:
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/SpaceWeatherColumns.png" alt="Space Weather Columns" title="Space Weather Columns" />

#### A description of these data fields can be found here: https://celestrak.com/SpaceData/SpaceWx-format.php
#### Note that the columns shown in the image have been renamed from the original dataset. 

### Climate Data 
#### Climate Data was taken from: https://www.ncdc.noaa.gov/
#### Data Description: The climate data used for this project includes monthly climate data ranging from 01/01/2000 - 12/31/2019 and contains weather data from 5 different weather stations including:
#### -London Corbin Airport, KY
#### -Jerome CO Airport, ID
#### -Salina Municipal Airport, KS
#### -Greenville Main Forestry Service, ME
#### -Annapolis NAF, MD
#### The climate data used for this project contains the following columns: 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/ClimateColumns.png" alt="Climate Columns" title="Climate Columns" />

#### Note that the columns above still need to be identified and cleaned to make sense. 

## Final Climate and Space Weather Data
#### The Space Weather Data is a subset of the original data as shown below:
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/SpaceWeatherSubset.png" alt="Subset of Space Weather" title="Subset of Space Weather" />

#### The Climate Data is a subset of the original data as show below: 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/ClimateSubset.png" alt="Subset of Climate Data" title="Subset of Climate Data" />

#### Both the Space Weather Data and the Climate data were indexed by Year and Month and then merged as shown below: 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/MergedSpaceClimateData.png" alt="Merged Data" title="Merged Data" />

### Average Wind Speed from Merged Data
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/MergedDataGraph.png" alt="Merged Data" title="Merged Data" />

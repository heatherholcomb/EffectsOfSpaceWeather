# EffectsOfSpaceWeather
## High Level Description
##### Space Weather describes the variations in the space environment between the sun and earth. In particular, Space Weather describes the phenomena that impact systems and technologies in orbit and on Earth. Space Weather can occur anywhere from the surface of the sun to the surface of the earth. 
##### Different aspects of space weather can affect multiple systems here on earth such as GPS, Climate, Radio and Satellite Communication. Solar flares can affect radio waves, solar energetic particles can cause electrical failure in satellites and block radio communications, geomagnetic storms can modify systems from GPS, when cosmic rays are high it can create nucleation in the atmosphere and produce more cloudy conditions and solar irradiance can have an affect on climate as well. 
##### The questions i would like to answer with this project include:  
###### - How does the Kp Index, or geomagnetic activity effect climate? 
###### - How does the F10.7 index effect climate? 
###### - How does Ap - Planetary Equivalent Amplitude effect climate? 
###### - How does Cp - Planetary Daily Character Figure effect climate? 
###### - How does ISN - International Sunspot Number effect climate? 
###### - Can I predict space weather using historical data? 

## Kp Index 
### Description of Kp Index: 
#### The Kp-index is the global geomaagnetic activity index that is based on 3-hour measuremetns from ground-based magnetometers around the world. The value being used for the models described below is the Sum of the 8 Kp indices for the day expressed to the nearest third of a unit.
#### Simple Linear Regression model - How does the Kp index affect Wind? 

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/SimpleLinearRegressionWindKp.png" alt="How does Kp Index affect wind" title="How does Kp index affect wind" />

#### Simple Linear Regression - How does Kp index affect Temperature? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/SimpleLinearRegressionTempKp.png" alt="How does Kp Index affect temperature" title="How does Kp index affect temperature" />

## F10.7
### Description of F10.7: 
#### The F10.7 Index is a measure of the noise level generated by the sun at a wavelength of 10.7 cm at the earth's orbit. this index has been used as an input to ionospheric models as a surrogate for the solar output in wavelengths that produce photoionization in the earth's ionosphere (in the ultraviolet bands).

## Ap 
### Description of Ap Index 
#### The Ap-index provides a daily average level for geomagnetic activity. Because of the non-linear relationship of the K-scale to magnetometer fluctuations, it is not meaningful to take the average of a set of K-indices. Instead, every 3-hour K-value will be converted back into a linear scale called the a-index. The average from 8 daily a-values gives us the Ap-index of a certain day. The Ap-index is thus a geomagnetic activity index where days with high levels of geomagnetic activity have a higher daily Ap-value.

## Cp
### Description of Cp Index 
#### 

## ISN - International Sunspot Number

## Space Weather Predictions 
#### fbprophet forecast model of F10.7 index. It seems that the forecast values line up with the actual values which is why i decided to take a further look at predictions the F10.7 index.
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107Predictions.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### fbprophet forecast model for Sum Of Kp index. This graph doesnt tell me much. There are so many different values for the Sum Of Kps and there doesnt seem to be much of a trend but i decided to take a further look at predicting these values to see if it is possible. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KpPredictions.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Mean Resample of F10.7 Time series graph. This shows me that there might be some sort of trend over time. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107TimeSeries1.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Time series decomposition for F10.7 and Augmented Dickey Fuller test. There seems to be a trend in the data and the data appears to be stationary. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107TimeSeries2.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107_ADF.png" alt="F10.7 ADF Test" title="F10.7 ADF Test" />

#### Autocorrelation plot for F10.7. If i'm interpreting this plot correctly, F10.7 is positively correlated up to k=30 and negatively correlated from ~46 on. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107AutoCorrelation.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Partial autocorrelation plot. F10.7 has significat partial autocorrelation at 2,4,11,12,13,23,26,27. I'm not seeing any pattern in the periods. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107PartialAutoCorrelation.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

### F10.7 ARIMA Model
#### Based on the Auto Correlation and Partial Auto Correlation plots, i played around with the order for my ARIMA Model and found AR = 4, Differencing Order = 0 and Moving Average = 2 was the best fit for this model. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107ARIMAModelCode.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107ARIMAModelGraph1.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### As you can see from the graph below, predicting out to ~2040, the forecast seems to follow the pattern of the data. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107ARIMAModelGraph2.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Next i'm going to show the results from the ARIMA model and plot the residuals to ensure that we have constant mean and variance
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107ARIMAModelResults.png" alt="F10.7 Predictions" title="F10.7 Predictions" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107ARIMAModelGraph3.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### The Residual graph shows a near zero mean and uniform variance. 
#### Finally we will look at Mean Absolute Percentage Error and Root Mean Square Error to see how accurate this model is 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107ARIMAModelStats.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### An MAPE value of 7.24% means that the model is about 92.76% accurate in predicting the next 15 observations. 
#### An RMSE value of 14.59 tells me that the model was able to forecast the F10.7 value within 14.59. 

### SARIMAX Model
#### Results Summary
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARIMAXModel2.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### SARIMAX Residuals
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARIMAXModel1.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### SARIMAX Model predictions for F10.7. The one step ahead forecast seems to match up nicely with the observed values showing me that this might be a good model to predict F10.7. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107Predictions2.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Mean Squared Error
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107MSE.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Root Mean Squared Error
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107RMSE.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

## References: 
###### https://www.swpc.noaa.gov/
###### https://celestrak.com/
###### https://www.ncdc.noaa.gov/
###### https://www.spacewx.com/Definitions.html#F10
###### https://www.spaceweatherlive.com/en/help/the-kp-index
###### https://spawx.nwra.com/spawx/f10.html
###### https://www.spaceweatherlive.com/en/help/the-ap-index


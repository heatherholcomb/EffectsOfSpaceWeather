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

#### Simple Linear Regression - How does Kp index affect Temperature? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/SimpleLinearRegressionTempKp.png" alt="How does Kp Index affect temperature" title="How does Kp index affect temperature" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Kp_Temp.png" alt="How does Kp Index affect temperature" title="How does Kp index affect temperature" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between the Kp Index and Average Temperature
#### H1: There is a Linear relationship between the Kp Index and Average Temperature

#### To accept or reject the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Kp_Temp.png" alt="How does Kp Index affect temperature" title="How does Kp index affect temperature" />

#### Simple Linear Regression model - How does the Kp index affect Wind Speed? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/SimpleLinearRegressionWindKp.png" alt="How does Kp Index affect wind" title="How does Kp index affect wind" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Kp_Wind.png" alt="How does Kp Index affect wind" title="How does Kp index affect wind" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between the Kp Index and Average Wind Speed
#### H1: There is a Linear relationship between the Kp Index and Average Wind Speed

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Kp_Wind.png" alt="How does Kp Index affect wind" title="How does Kp index affect wind" />

#### Simple Linear Regression Model - How does the Kp index affect Precipitation? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_Kp_Precip.png" alt="How does Kp Index affect precipitation" title="How does Kp index affect precipitation" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Kp_Precip.png" alt="How does Kp Index affect precipitation" title="How does Kp index affect precipitation" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between the Kp Index and Precipitation
#### H1: There is a Linear relationship between the Kp Index and Precipitation

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Kp_Precip.png" alt="How does Kp Index affect precipitation" title="How does Kp index affect precipitation" />

## F10.7
### Description of F10.7: 
#### The F10.7 Index is a measure of the noise level generated by the sun at a wavelength of 10.7 cm at the earth's orbit. this index has been used as an input to ionospheric models as a surrogate for the solar output in wavelengths that produce photoionization in the earth's ionosphere (in the ultraviolet bands).

#### Simple Linear Regression model - How does F10.7 affect Temperature? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_F107_Temp.png" alt="How does F10.7 affect temperature" title="How does F10.7 affect temperature" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_F107_Temp.png" alt="How does F10.7 affect temperature" title="How does F10.7 affect temperature" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between F10.7 and Average Temperature
#### H1: There is a Linear relationship between F10.7 and Average Temperature

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_F107_Temp.png" alt="How does F10.7 affect temperature" title="How does F10.7 affect temperature" />


#### Simple Linear Regression model - How does F10.7 affect Wind Speed? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_F107_Wind.png" alt="How does F10.7 affect wind" title="How does F10.7 affect wind" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_F107_Wind.png" alt="How does F10.7 affect wind" title="How does F10.7 affect wind" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between F10.7 and Average Wind Speed
#### H1: There is a Linear relationship between F10.7 and Average Wind Speed

#### To accept or reject the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_F107_Wind.png" alt="How does F10.7 affect wind" title="How does F10.7 affect wind" />


#### Simple Linear Regression model - How does F10.7 affect Precipitation?
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_F107_Precip.png" alt="How does F10.7 affect precipitation" title="How does F10.7 affect precipitation" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_F107_Precip.png" alt="How does F10.7 affect precipitation" title="How does F10.7 affect precipitation" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between F10.7 and Precipitation
#### H1: There is a Linear relationship between F10.7 and Precipitation

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_F107_Precip.png" alt="How does F10.7 affect precipitation" title="How does F10.7 affect precipitation" />

## Ap 
### Description of Ap Index 
#### The Ap-index provides a daily average level for geomagnetic activity. Because of the non-linear relationship of the K-scale to magnetometer fluctuations, it is not meaningful to take the average of a set of K-indices. Instead, every 3-hour K-value will be converted back into a linear scale called the a-index. The average from 8 daily a-values gives us the Ap-index of a certain day. The Ap-index is thus a geomagnetic activity index where days with high levels of geomagnetic activity have a higher daily Ap-value.

#### Simple Linear Regression model - How does the Ap index affect Temperature? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_Ap_Temp.png" alt="How does Ap affect temperature" title="How does Ap affect temperature" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Ap_Temp.png" alt="How does Ap affect temperature" title="How does Ap affect temperature" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between Ap Index and Average Temperature
#### H1: There is a Linear relationship between Ap Index and Average Temperature

#### To accept or reject the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Ap_Temp.png" alt="How does Ap affect temperature" title="How does Ap affect temperature" />

#### Simple Linear Regression model - How does the Ap index affect Wind Speed? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_Ap_Wind.png" alt="How does Ap affect wind" title="How does Ap affect wind" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Ap_Wind.png" alt="How does Ap affect wind" title="How does Ap affect wind" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between Ap Index and Average Wind Speed
#### H1: There is a Linear relationship between Ap Index and Average Wind Speed

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModel_Ap_Wind.png" alt="How does Ap affect wind" title="How does Ap affect wind" />

#### Simple Linear Regression model - How does the Ap index affect Precipitation?
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_Ap_Precip.png" alt="How does Ap affect precipitation" title="How does Ap affect precipitation" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Ap_Precip.png" alt="How does Ap affect precipitation" title="How does Ap affect precipitation" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between Ap Index and Precipitation
#### H1: There is a Linear relationship between Ap Index and Precipitation

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Ap_Precip.png" alt="How does Ap affect precipitation" title="How does Ap affect precipitation" />

## Cp
### Description of Cp Index 
#### 

#### Simple Linear Regression model - How does the Cp index affect Temperature? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_Cp_Temp.png" alt="How does Cp affect temperature" title="How does Cp affect temperature" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Cp_Temp.png" alt="How does Cp affect temperature" title="How does Cp affect temperature" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between Cp Index and Average Temperature
#### H1: There is a Linear relationship between Cp Index and Average Temperature

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Cp_Temp.png" alt="How does Cp affect temperature" title="How does Cp affect temperature" />


#### Simple Linear Regression model - How does the Cp index affect Wind Speed? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_Cp_Wind.png" alt="How does Cp affect wind" title="How does Cp affect wind" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Cp_Wind.png" alt="How does Cp affect wind" title="How does Cp affect wind" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between Cp Index and Average Wind Speed
#### H1: There is a Linear relationship between Cp Index and Average Wind Speed

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Cp_Wind.png" alt="How does Cp affect wind" title="How does Cp affect wind" />


#### Simple Linear Regression model - How does the Cp index affect Precipitation? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_Cp_Precip.png" alt="How does Cp affect precipitation" title="How does Cp affect precipitation" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_Cp_Precip.png" alt="How does Cp affect precipitation" title="How does Cp affect precipitation" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between Cp Index and Precipitation
#### H1: There is a Linear relationship between Cp Index and Precipitation

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_Cp_Precip.png" alt="How does Cp affect precipitation" title="How does Cp affect precipitation" />


## ISN - International Sunspot Number
### Description of ISN
####

#### Simple Linear Regression model - How does ISN affect Temperature? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_ISN_Temp.png" alt="How does ISN affect temperature" title="How does ISN affect temperature" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_ISN_Temp.png" alt="How does ISN affect temperature" title="How does ISN affect temperature" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between ISN Index and Average Temperature
#### H1: There is a Linear relationship between ISN Index and Average Temperature

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_ISN_Temp.png" alt="How does ISN affect temperature" title="How does ISN affect temperature" />


#### Simple Linear Regression model - How does ISN affect Wind Speed? 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_ISN_Wind.png" alt="How does ISN affect wind" title="How does ISN affect wind" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_ISN_Wind.png" alt="How does ISN affect wind" title="How does ISN affect wind" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between ISN Index and Average Wind Speed
#### H1: There is a Linear relationship between ISN Index and Average Wind Speed

#### To accept or reject the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_ISN_Wind.png" alt="How does ISN affect wind" title="How does ISN affect wind" />


#### Simple Linear Regression model - How does ISN affect Precipitation?
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearRegression_ISN_Precip.png" alt="How does ISN affect precipitation" title="How does ISN affect precipitation" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinearModelPlot_ISN_Precip.png" alt="How does ISN affect precipitation" title="How does ISN affect precipitation" />

#### Looking at the plot above, there seems to be no linear relationship between the two variables. So our null and alternative hypothesis are as follows: 
#### H0: There is no Linear relationship between ISN Index and Precipitation
#### H1: There is a Linear relationship between ISN Index and Precipitation

#### To accept or deny the null hypothesis, i split the data into test and training sets, fit a linear regression model and looked at the Mean Squared Error as well as the coefficient
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/LinModelFinal_ISN_Precip.png" alt="How does ISN affect precipitation" title="How does ISN affect precipitation" />

## Space Weather Predictions 
#### fbprophet forecast model of F10.7 index. It seems that the forecast values line up with the actual values which is why i decided to take a further look at predictions the F10.7 index.
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107Predictions.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### fbprophet forecast model for Sum Of Kp index. This graph doesnt tell me much. There are so many different values for the Sum Of Kps and there doesnt seem to be much of a trend but i decided to take a further look at predicting these values to see if it is possible. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KpPredictions.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

### F10.7 Prediction

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

### F10.7 SARIMAX Model
#### Based on the partial auto correlation plot, i used the same values for this model as i did in the ARIMA model. AR = 4, Differencing order = 0 and Moving Average = 2
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARModel.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Prediction Plot - Based on the prediction plot below, the forecast values seem to follow the pattern of the data. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARModelPredictionGraph.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### Next i'm going to show the results from the SARIMAX model and plot the residuals to ensure that we have constant mean and variance 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARModelResults.png" alt="F10.7 Predictions" title="F10.7 Predictions" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARModelResiduals.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### The residuals grpah shows a near zero mean and uniform variance 
#### Finally, we will look at Mean Absolute Percentage Error and Root Mean Square Error to see how accurate this model is
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARModelMAPE.png" alt="F10.7 Predictions" title="F10.7 Predictions" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/F107SARModelRMSE.png" alt="F10.7 Predictions" title="F10.7 Predictions" />

#### A MAPE value of 10% means that the model is about 90% accurate in predicting the next 15 observations. 
#### An RMSE value of24.13 tells me that the model was able to forecast the F10.7 values within 24.13. 

### SumOfKps Prediction
#### Mean Resample of Sum Of Kps Time series graph. This shows me that there might be some sort of trend over time. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPTimeSeries.png" alt="Kp Predictions" title="Kp Predictions" />

#### Time series decomposition for Kp and Augmented Dickey Fuller test. There seems to be a trend in the data and the data appears to be stationary. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPDecomposition.png" alt="Kp Predictions" title="Kp Predictions" />

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPADF.png" alt="Kp Predictions" title="Kp Predictions" />

#### Autocorrelation plot for Kp. If i'm interpreting this plot correctly, Kp is positively correlated. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPAutoCorrelation.png" alt="Kp Predictions" title="Kp Predictions" />

#### Partial autocorrelation plot. Kp has significat partial autocorrelation at 1,2,4,5,6,10,11,12. I'm not seeing any pattern in the periods. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPPartialAutoCorrelatino.png" alt="Kp Predictions" title="Kp Predictions" />

### SumOfKps ARIMA Model 
#### Based on the Auto Correlation and Partial Auto Correlation plots, i played around with the order for my ARIMA Model and found AR = 6, Differencing Order = 0 and Moving Average = 2 was the best fit for this model. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPARIMAModelCode.png" alt="Kp Predictions" title="Kp Predictions" />
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPARIMAModelGraph.png" alt="Kp Predictions" title="Kp Predictions" />

#### Plotting the predictions, this model seems to predict well for a short period of time 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPARIMAModelGraph1.png" alt="Kp Predictions" title="Kp Predictions" />

#### Next i'll show the Kp ARIMA model results and plot the residuals to ensure that we have constant mean and variance
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPARIMAModelResults.png" alt="Kp Predictions" title="Kp Predictions" />

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPARIMAModelResiduals.png" alt="Kp Predictions" title="Kp Predictions" />

#### The residual errors have a near zero mean and uniform variance 

#### Lastly we will look at Mean Absolute Percentage Error and Root Mean Square Error to see how accurate this model is
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KPARIMAModelErrors.png" alt="Kp Predictions" title="Kp Predictions" />

#### A MAPE value of 13.25 means that the model is about 86.75% accurate in predicting the next 15 observations. 
#### An RMSE tells me that the model was able to forecast SumOfKps within 27.811. 

### SumOfKps SARIMAX Model 
#### Based on the partial auto correlation plot, i used the same values for this model as i did the ARIMA model. AR = , Differencing Order = , Moving Average = 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KpSARModel.png" alt="Kp Predictions" title="Kp Predictions" />

#### This prediction plot doesnt seem to accurately predict the values but does seem to follow the pattern of the data. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KpSARPredictionPlot.png" alt="Kp Predictions" title="Kp Predictions" />

#### Next i will show the Kp SARIMAX model results and plot the residuals to ensure that we have constant mean and variance. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KpSARResults.png" alt="Kp Predictions" title="Kp Predictions" />

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KpSARResiduals.png" alt="Kp Predictions" title="Kp Predictions" />

#### The residual errors have a near zero mean and uniform variance
#### Finally we will look at Mean Absolute Percentage Error and Root Mean Square Error to see how accurate this model is
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/KpSARErrors.png" alt="Kp Predictions" title="Kp Predictions" />

#### The MAPE Value of 16.51% means that the model is about 83.49% accurate at predicting the next 15 observations.
#### The RMSE tells me that my model was able to forecast the Kp Index within 40.39 of the real values. 

### Model Comparison 
#### Looking at the error comparisons below, it shows that the ARIMA model has a lower MAPE and a lower RMSE which means it performed better than the SARIMAX model in both instances. 
<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/MAPEComparison.png" alt="MAPE Comparison" title="MAPE Comparison" />

<img src="https://github.com/heatherholcomb/EffectsOfSpaceWeather/blob/master/Images/RMSEComparison.png" alt="RMSE Comparison" title="RMSE Comparison" />

## References: 
###### https://www.swpc.noaa.gov/
###### https://celestrak.com/
###### https://www.ncdc.noaa.gov/
###### https://www.spacewx.com/Definitions.html#F10
###### https://www.spaceweatherlive.com/en/help/the-kp-index
###### https://spawx.nwra.com/spawx/f10.html
###### https://www.spaceweatherlive.com/en/help/the-ap-index


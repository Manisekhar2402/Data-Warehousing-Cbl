# Concept Based Learning on Data Warehousing

Now a day’s people are turning up to airways to get their works done faster prior to the remaining ways this is due to wide variety of reasons such as time, comfort, offers given by the airlines. We are going to predict the air fare in 4th quarter of 2014.  
We have a data set of 2012, 2013, and 2014. Each year consist of 4 quarter’s. Each quarter consist of 14 attributes and 1000 observations. In the data set 2 are nominal variables and 12 are numeric variables

Step1: Firstly we have to find what are the important and more considered attributes in the Training data.
Step2: Fitting the model
	times1<-ts(omittemp,frequency=4, start=c(2012,1),end=c(2014,3))
	dtimes1<-decompose(times1)
	dtimes1$seasonal 
	finalfit<-auto.arima(times)
Step4:  Then after fitting the model predict the result for the test data using Predict Function.
finalforcast <- forecast.Arima(finalfit, h=1000)

---
title: "Milestone1"
author: "Margot Chen, Qi Yang"
date: "2020/02/27"
always_allow_html: true
output: 
  html_document:
    keep_md: yes
    toc: true
---



## Beijing PM2.5   
### Introduction  
Beijing, the capital city of China, is fighting against __PM2.5__ pollution in recent years. PM2.5 refers to fine airborne particles with a diameter of 2.5μm or less. They can cause severe damage to human health by triggering lung cancer, heart diseases, stroke, and respiratory infections. A Nature study pointed out that in 2016 only, PM2.5 was associated with over four million deaths worldwide. In the past decades, the air quality in Beijing has been faced with great pressure resulting from the rapid development of industry. In order to secure its citizens’ health, Chinese government has taken action to mitigate the influence of PM2.5 since 2012.      
Previous studies showed that __meteorological conditions__, such as wind and humidity, could contribute to the formation of PM2.5. Therefore, we speculate that there could be correlations between Beijing’s PM2.5 concentration([PM2.5]) and the meteorological conditions in a sufficient period of time. If so, knowing the meteorological conditions can support the assessment and even prediction of air quality in Beijing. 
 
### Data Description  
The [dataset](https://archive.ics.uci.edu/ml/datasets/Beijing+PM2.5+Data#) used in our project was obtained from University of California Irvine Machine learning Repository. It was originally uploaded by Songxi Chen in Peking University, China. It is an hourly dataset containing 1) the __[PM2.5]__ of US Embassy in Beijing and 2) __meteorological statistics__ from Beijing Capital International Airport. The data was collected from Jan 1st, 2010 to Dec 31st, 2014. The original purpose of the dataset was to assess the effect of Chinese government’s pollution reduction plan which started from 2012.    

Below are the variables in the dataset:    

| Variable          | Type             | Description | 
|-------------------|------------------|-------------|
| year              | Quantitative     |Year of data in this row|
| month             | Quantitative     |Month of data in this row|
| day               | Quantitative     |Day of data in this row|
| hour              | Quantitative     |Hour of data in this row|
| pm2.5             | Quantitative     |PM2.5 concentration (ug/m^3)|
| DEWP              | Quantitative     |Dew Point (â„ƒ)|
| TEMP              | Quantitative     |Temperature (â„ƒ)|
| PRES              | Quantitative     |Pressure (hPa)|
| cbwd              | Categorical      |Combined wind direction|
| lws               | Quantitative     |Cumulated wind speed (m/s)|
| ls                | Quantitative     |Cumulated hours of snow|
| lr                | Quantitative     |Cumulated hours of rain|

### Dataset loading



### Dataset exploration   
1.	We are interested in the correlation between meteorological conditions (dew point, temperature and pressure) and [PM2.5]. Thus, we created a __scatterplot__ of _[FILL HERE: a meteorological condition] VS. [PM2.5]_.
2.	Wind is one of the important elements of weather conditions, and could also influence the formation of PM2.5. Therefore, we used a __faceted scatterplot__ in order to check the correlation between _wind speed and [PM2.5] for different wind directions_ (northwest, northeast, southwest and southeast).
3.	In addition to meteorological conditions, we are curious about the potential influence of _time on [PM2.5]_, so we created a __heat map__ showing [PM2.5] in different hours and months. 
4.	We also create a __histogram__ emphasizing the severity of _PM2.5 in different seasons_.
5.	In order to check the effect of PM2.5 reduction plan initiated by Chinese government in 2012, we generated a __line chart__ showing _how PM2.5 changes across years_.

### Research Question    
Our main research question is an _exploratory_ question: does the [PM2.5] in Beijing correlates with meteorological conditions and time? Sub-questions as below are also _exploratory_ as they all focus on the correlation between [PM2.5] and a certain variable.    
-	[PM2.5] VS. physical parameters (dew point, temperature and pressure).    
-	[PM2.5] VS. wind.     
-	[PM2.5] VS. special weather conditions (rain and snow).     
-	[PM2.5] VS. time (year, month, a time in a day).    

### Plan of Action   
1.	Deal with missing values.
2.	Run tests of correlation between [PM2.5] and meteorological statistics/time.
3.	Perform a linear regression analyses and plot quantitative variables in a regression line.
4.	Demonstrate the correlation between [PM2.5] and categorical variables. Only wind direction is a categorical variable at first, but categorical time units (season, day or night) can also be adapted from quantitative records.
5.	Create an interactive dashboard showing potential correlations between meteorological conditions/time and [PM2.5].
6.	Address the effectiveness of Chinese government’s action on solving air quality issues.

### References
Liang, X., Zou, T., Guo, B., Li, S., Zhang, H., Zhang, S., Huang, H. and Chen, S. X. (2015). Assessing Beijing's PM2.5 pollution: severity, weather impact, APEC and winter heating. Proceedings of the Royal Society A, 471, 20150257.
# Prediting-traffic-flow-of-Orange-County

# Overview and Motivation
For intelligent transportation systems (ITS), it is necessary to have information about the actual and near-future traffic volume. That is why traffic volume prediction is a critical element of traffic flow management and operation. The transport authorities can use the insights from traffic volume prediction to avoid congestion on roadways. For everyday drivers, real-time estimates of traffic flow can provide knowledge and direction to enhance their travel experience and reduce costs. 

On daily traffic, the weather may have an impact on travel time and traffic flow. Especially, inclement weather can significantly degrade roadway traffic operations. Traffic flow is also dependent on the day of a week, that is, if the day is a weekend, holiday, or weekday and which part of the day it is.  Moreover, we saw a large drop in traffic volume after the start of the COVID-19 lockdown.  In this project, I will use linear regression and random forest to estimate future traffic flow based on weather conditions in Orange county Florida. I also incorporate the effect of the pandemic on traffic volume. 

# Related Work
Due to the importance of traffic flow prediction in urban traffic optimization, predicting traffic flow is a very popular topic across academia. A lot of work has been done since the last century.  Some of the important approaches were proposed using time series models <sup>[1](#Billy)</sup> <sup>[2](#Said)</sup> <sup>[3](#Moorthy)</sup>, Kalman filter theory <sup>[4](#Iwao)</sup>, Markov chain model <sup>[5](#Guoqiang)</sup>, non-parametric methods <sup>[6](#Oswald)</sup>, Bayesian networks <sup>[7](#Enrique)</sup>, etc.  Moreover, in recent years, people are using deep learning to predict the traffic flow <sup>[8](#Lv)</sup> <sup>[9](#Tedjopurnomo)</sup>. 

For this project, I am mostly inspired by the work done on Metro Interstate Traffic Volume Data Set <sup>[10](#metro)</sup> <sup>[11](#manoj)</sup> <sup>[12](#ramyahr)</sup> <sup>[13](#simonwenkel)</sup>. 

# Initial Questions
Through this project, I seek to answer four primary questions:

* How do weather variables affect the traffic volume of Orange county?
* How do Covid-19 affect the traffic volume of Orange county?
* What is the effect of different holidays and different part of the day on the traffic volume of Orange county?
* How we can use the variable to predict the traffic volume of Orange county?

# Data
The hourly volume of traffic of orange county has been scrapped from the website of the [Florida Department of Transportation]. Due to the unavailability, data from January 01, 2020 to July 08, 2020 has been collected.  The weather data has been bought from the [VisualCrossing]. Moreover, the traffic volume may be depended on the holidays and weekends. [The data for holidays] has also been collected and put in a csv file. 

# References

[Florida Department of Transportation]: https://www.fdot.gov/statistics/trafficdata/default.shtm
[VisualCrossing]: https://www.visualcrossing.com/
[The data for holidays]: https://www.officeholidays.com/countries/usa/florida/2020

<a name="Billy">1</a>: M.ASCE Billy M. Williams and F.ASCE Lester A. Hoel. Modeling and forecasting vehicular traffic flow as a seasonal arima process: Theoretical basis and empirical results. Journal of Transportation Engineering, 129(6):664–672, November 2003.

<a name="Said">2</a>: Z.M.B. Said M.M. Hamed, H.R. Al-Masaeid. Short-term prediction of traffic volume in urban arterials. Journal
of Transportation Engineering, pages 249–254, 1995.

<a name="Moorthy">3</a>: C. K. Moorthy and B. G. Ratcliffe. Short term traffic forecasting using time series methods. Transportation
Planning and Technology, 12(1):45–56, 1988.

<a name="Iwao">4</a>: Iwao Okutani and Yorgos J. Stephanedes. Dynamic prediction of traffic volume through kalman filtering theory.
Transportation Research Part B: Methodological, 18(1):1 – 11, 1984.

<a name="Guoqiang">5</a>: Guoqiang Yu, Jianming Hu, Changshui Zhang, Like Zhuang, and Jingyan Song. Short-term traffic flow forecasting based on markov chain model. In Intelligent Vehicles Symposium, 2003. Proceedings. IEEE, pages 208 – 212, june 2003.

<a name="Oswald">6</a>: R.K. Oswald B.L. Smith, B.M. Williams. Parametric and nonparametric traffic volume forecasting. Paper
Presented at the 2000 Transportation Research Board Annual Meeting, Washington, DC, 2000.

<a name="Enrique">7</a>: Enrique Castillo, Jos Mara Menndez, and Santos Snchez-Cambronero. Predicting traffic flow using bayesian
networks. Transportation Research Part B: Methodological, 42(5):482 – 509, 2008

<a name="Lv">8</a>: Lv Y, Duan Y, Kang W, Li Z, Wang FY. Traffic flow prediction with big data: a deep learning approach. IEEE Transactions on Intelligent Transportation Systems. 2014 Sep 9;16(2):865-73.

<a name="Tedjopurnomo">9</a>: Tedjopurnomo DA, Bao Z, Zheng B, Choudhury F, Qin AK. A Survey on Modern Deep Neural Network for Traffic Prediction: Trends, Methods and Challenges. IEEE Transactions on Knowledge and Data Engineering. 2020 Jun 9.

<a name="metro">10</a>: https://archive.ics.uci.edu/ml/datasets/Metro+Interstate+Traffic+Volume

<a name="manoj">11</a>: https://github.com/ManojKumarMaruthi/Regression

<a name="ramyahr">12</a>: https://www.kaggle.com/ramyahr/metro-interstate-traffic-volume

<a name="simonwenkel">13</a>: https://www.simonwenkel.com/2019/06/20/revisitingML-Metro-Interstate-Traffic_volume.html

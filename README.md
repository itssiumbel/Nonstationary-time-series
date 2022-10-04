# Project 1
In accordance with [the objective of this project](https://github.com/itssiumbel/Nonstationary-time-series/blob/main/Objective%20and%20Purposes.pdf), which consists in highlighting the trend from nonstationary time series, I performed the following tasks:

1. Collected a data representing a deliberately nonstationary time series and then considered various types of trends: a) linear, b) exponential,
c) logarithmic, e) quadratic, e) power. Using the least squares method,I found the coefficients of the equations, substituted them into the trend equations. And then it became possible to highlight the trends from the data and obtain the residuals. Below presented plots of the linear and quadratic trend equations.
*************
![The plot of the linear trend equation.](https://github.com/itssiumbel/Nonstationary-time-series/blob/main/%D0%BB%D0%B8%D0%BD%D0%B5%20%D1%82%D1%80%D0%B5%D0%BD%D0%B4.PNG)
![The plot of the quadratic trend equation.](https://github.com/itssiumbel/Nonstationary-time-series/blob/main/%D0%BA%D0%B2%D0%B0%D0%B4%D1%80%D0%B0%D1%82%D0%B8%D1%87%D0%BD%D1%8B%D0%B9%20%D1%82%D1%80%D0%B5%D0%BD%D0%B4.PNG)
**************
2. Here was the step where I analysed the residuals and checked them for stationarity by obtaining autocorrelation matrix and its eigen values. It was found that the nonstationary series after the trend highlighting becomes stationary, which can be considered as success. Next I obtained a model for further fitting of the residuals. In addition, autocorrelation and partial autocorrelation functions were constructed, according to their behavior I made an assumption that the model would be MA(2) and AR(1).
***********
![The plot of the autocorrelation function.](https://github.com/itssiumbel/Nonstationary-time-series/blob/main/%D0%B3%D1%80%D0%B0%D1%84%D0%B8%D0%BA%20%D0%B0%D0%B2%D1%82%D0%BE%D0%BA%D0%BE%D1%80%D1%80%D0%B5%D0%BB%D1%8F%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D0%BE%D0%B9%20%D1%84%D1%83%D0%BD%D0%BA%D1%86%D0%B8%D0%B8.PNG)
![The plot of the partial autocorrelation function.](https://github.com/itssiumbel/Nonstationary-time-series/blob/main/%D0%B3%D1%80%D0%B0%D1%84%D0%B8%D0%BA%20%D1%87%D0%B0%D1%81%D1%82%D0%BD%D0%BE%D0%B9%20%D0%B0%D0%B2%D1%82%D0%BE%D0%BA%D0%BE%D1%80%D1%80%D0%B5%D0%BB%D1%8F%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D0%BE%D0%B9%20%D1%84%D1%83%D0%BD%D0%BA%D1%86%D0%B8%D0%B8.PNG)
***************

3. On this step I tested an alternative method of obtaining residuals. The issue in order to find out whether it is possible to identify a trend in a time series without resorting to a method that includes certain equations with specially selected coefficients. As the plot of the autocorrelation function shows us, this method is successful and suitable for use.
 ***********
![The plot of the alternative autocorrelation function.](https://github.com/itssiumbel/Nonstationary-time-series/blob/main/%D0%B3%D1%80%D0%B0%D1%84%D0%B8%D0%BA%20%D0%B0%D0%B2%D1%82%D0%BE%D0%BA%D0%BE%D1%80%D1%80%D0%B5%D0%BB%D1%8F%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D0%BE%D0%B9%20%D1%84%D1%83%D0%BD%D0%BA%D1%86%D0%B8%D0%B8%20%D0%B4%D0%BB%D1%8F%20%D0%B0%D0%BB%D1%8C%D1%82%D0%B5%D1%80%D0%BD%D0%B0%D1%82%D0%B8%D0%B2%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BC%D0%B5%D1%82%D0%BE%D0%B4%D0%B0.PNG)
***************

4. I fitted tha data with various models _(AR(p), MA(q), ARMA(pq))_. And after obtaining a new time series – the final fit, it was compared with the original data by  mean square error, which shows the level of the quality of the data approximation, and, therefore, the quality of the fit.

5. Based on the results of the comparative analysis, it was concluded that the best model for fitting the data is MA(1), which, however, contradicts the assumption about the model, which was made on the behavior of the autocorrelation function and the partial autocorrelation function. In addition, it was concluded that the residuals obtained from some types of trends (linear and logarithmic) fit better of the rest, which means that these trends are preferable in use in practice.


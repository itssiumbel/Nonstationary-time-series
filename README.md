In accordance with the objective of this project ("Objective and Purposes" pdf file), which consists in highlighting the trend from nonstationary time series, the following tasks were performed:

1. Data representing a deliberately nonstationary time series were collected, and then various types of trends were considered: a) linear, b) exponential,
c) logarithmic, e) quadratic, e) power. Using the least squares method, the coefficients of the equations I found, substituted them into the trend equations. And then it became possible to isolate the trends themselves from the data and obtain the residuals.

2. On this step I tested an alternative method of obtaining residues. The issue in order to find out whether it is possible to identify a trend in a time series without resorting to a method that includes certain equations with specially selected coefficients. As we can see, this method is successful and suitable for use.

3. When the residues were analyzed and checked for stationarity, we determined a model for further fitting of the residues. In the RStudio I built an autocorrelation matrix and it was certain that only with its positive certainty, the time series under study is stationary. It can be seen that the non-stationary series after the trend highlighting becomes stationary, which can be considered as success. In addition, autocorrelation and partial autocorrelation functions were constructed, according to the behavior of which the assumption about the model was made the fits are MA(2) and AR(1).

4. Then the fitting was done with various models, the functions for which were pre-programmed in RStudio. After obtaining a new time series – the final fit, it was compared with the original data by means of a standard error, which shows the level of the quality of the data approximation, and, therefore, the quality of the fit.

5. Based on the results of the comparative analysis, it was concluded that the best model for fitting the data is MA(1), which, however, contradicts the assumption about the model, which was made on the behavior of the autocorrelation function and the partial autocorrelation function. In addition, it was concluded that the residuals obtained from some types of trends (linear and logarithmic) fit better of the rest, which means that these trends are preferable in use in practice.

Thus, all the tasks of this research work have been done, the goal has been achieved, and the hypothesis has been confirmed.

# Energy-consumption-metering-and-forecasting


Development of a machine learning based model to predict energy consumption in an university campus environment in real time. Time series forecasting is one of the most important topics in data science. We needs to predict the future consumption in order to make better decisions and allocate resources more effectively.

## Data Acquisition 
The datasets that was used for the development of the machine learning model are available in https://github.com/FatimaAABADI/Energy-consumption-metering-and-forecasting/tree/main/Data

## Data description
The data of 4 smart meters corresponding to 4 different profils is used in this study.

The energy consumption of every 15 minutes, for 11 months (27-07-2017/04-07-2018) has been used.

## SVR Model
Support Vector Machines (SVM) are popularly and widely used for classification problems in machine learning.The use of SVMs in regression are known as Support Vector Regression (SVR).

SVR gives us the flexibility to define how much error is acceptable in our model and will find an appropriate line (or hyperplane in higher dimensions) to fit the data.

The objective function of SVR is to minimize the coefficients — more specifically, the l2-norm of the coefficient vector — not the squared error. 

Minimize: 

![This is an image](https://miro.medium.com/max/456/1*6M8yyY7yC7xJX6nFN2SdCQ.png)

Constraints:  

![This is an image](https://miro.medium.com/max/506/1*gpN_ZxDuLgusn-O0fck13A.png)


Illustrative Example:

![This is an image](https://miro.medium.com/max/1400/1*nrXHNqC_hqpyux7GUbtqAQ.png)


## Results

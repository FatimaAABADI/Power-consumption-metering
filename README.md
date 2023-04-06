# Power-consumption-metering

## Data Acquisition 
The datasets that are available in https://github.com/FatimaAABADI/Energy-consumption-metering-and-forecasting/tree/main/Data are extracted from a platform implemented in an university campus(INPT).

INPT ("Institut National des Postes et Télécommunications") stands for the National Institute of Posts and Telecommunications1. It is a Moroccan public Engineering School offering multiple curricula in information and communication technologies, and located in Rabat, the administrative capital of Morocco (North Africa). 

We implanted a simple yet reliable network consisting in 18 Schneider PM1200 Smart Meters under the authority of a Programmable Logic Controller (PLC), which is in turn connected to the Supervision Station through a gateway (for protocol translation). The Supervision Station in our control room displays in real time power consumption trends, every 15 minutes

![This is an image](https://miro.medium.com/max/456/1*6M8yyY7yC7xJX6nFN2SdCQ.png)










## Data description

The energy consumption of every 15 minutes, for 11 months has been used.

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

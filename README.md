# Power-consumption-metering

## Data Acquisition 
The datasets that are available in https://github.com/FatimaAABADI/Energy-consumption-metering-and-forecasting/tree/main/Data are extracted from a platform implemented in an university campus(INPT).

INPT ("Institut National des Postes et Télécommunications") stands for the National Institute of Posts and Telecommunications1. It is a Moroccan public Engineering School offering multiple curricula in information and communication technologies, and located in Rabat, the administrative capital of Morocco (North Africa). 

We implanted a simple yet reliable network consisting in 18 Schneider PM1200 Smart Meters under the authority of a Programmable Logic Controller (PLC), which is in turn connected to the Supervision Station through a gateway (for protocol translation). The Supervision Station in our control room displays in real time power consumption trends, every 15 minutes

![This is an image](https://github.com/FatimaAABADI/Power-consumption-metering/blob/main/img/bus%20(1).PNG)

We have installed:
1. 01 Vijeo citect 5000 points Supervision Station. It is a monitoring and control component of PlantStruxure™PES (Process Expert System). It provides configuration tools and features to consolidate and streamline control from an array of inputs (counted as "points").

2. 01 Switch for the Local Area Ethernet TCP/IP Network.

3. 01 Modicon M340 Programmable logic controller acting as a Master to collect data every 15 min. from the Smart Meters. This PLC serves also as a gateway to translate the Modbus-RTU protocol (IoT dedicated) into Ethernet TCP/IP. Moreover, in the case of future electrical equipment in- stallation (e.g., solar panels, other loads) it can act as a Smart Controller (e.g., for load shifting, solar/utility choice).

4. 12 on/off input and 8 on/off output modules. The Remote inputs/outputs are used for voltage supervision and horn control in case of a fault.

5. 01 EGX150, Ethernet Gateway to translate the Modbus RTU signal into Ethernet TCP/IP.

6. 01 Smart Meter for monitoring the electrical quantities of the Main low voltage Distribution Board (MDB) dedicated to student rooms.

7. 01 EGX150 reserve unit for future use.

8. 11 Smart Meters for monitoring the electrical quantities of the building C MDB.

9. 06 Smart Meters for monitoring the electrical quantities of the transformation station MDB.


Figure below presents specifically each Smart Meter’s monitoring area:

![This is an image](https://github.com/FatimaAABADI/Power-consumption-metering/blob/main/img/bus%20(1).PNG)


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

# Power-consumption-metering

[![DOI](https://zenodo.org/badge/553015219.svg)](https://zenodo.org/badge/latestdoi/553015219)

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

![This is an image](https://github.com/FatimaAABADI/Power-consumption-metering/blob/main/img/18%20compteurs.PNG)

Smart Meters PM 13, 14, 15,16 measure the electrical consumption in the different floors of the Dormitory 3. The Smart Meters PM 3,4 monitor Building B. PM 1 monitor building C. The Smart Meters PM 7, 8,9 are in charge of Dormitories 1 and 2. The Smart Meters PM 5,10,17 are in charge of Building D and E. PM 6,7, 11 are in charge of solar and lighting.

• Building A: Administration and services.

• Building B: Offices and classrooms.

• Building C: Library and auditorium.

• Building D: Labs and offices.

• Building E: Lecture Halls.

• Dormitories. One of them is home to the restaurant on the ground floor (
dormitory 1).

## Data description

The data is extracted from the infrastructure presented in the previous subsection. We collected 11 months of power consumption data from 16 Smart meters, with a 15 minutes granularity.

The outputs of this platform are: Date, Time, Current, Active Power ("useful" power in kW), Reactive Power ("useless" power bouncing from
source to load in Voltage Ampere Reactive), Apparent Power (combination of active and reactive power in Volt Amperes), Voltage and Power factor.

Figure below graphically represents each Smart Meter’s (PMX with X from 01 to 16) power consumption dataset. The X axis designates the 15 minute sample number (in chronological order) and the Y axis the associated power consumption (active power) at that moment

![This is an image](https://github.com/FatimaAABADI/Power-consumption-metering/blob/main/img/dfs.png)



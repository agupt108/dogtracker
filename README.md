 
 Most dog trackers are really expensive + a subscription if gps tech. The cheaper non subscription modules are bluetooth, limiting their range to around 300 m. However, using **LoRa**, and **Arduino**, we can create a relatively inexpensive GPS tracker that sends location data to a server, processing it and sending it to a phone as a IOS push notifications. LoRa, or Long Range Radio, is a long range wireless data transfer technique that communicates up to 10-15 km on a standard model. Higher end models can communicate up to 716 km. The **RYLR890/96**(either is good) module by Reyax is a very good for this project, because it has a good range of 10-15 km. Two are neeed to make a wireless data transfer, in this case between a dog tracker module and a main module. The data that we will be transferring is the dog's location, which will be found using a GPS module (in this case **GPS Neo-6M, GT-U7, around $12.97 from Amazon**). This data will be send through the LoRa module to the LoRa reciever which will upload the data on the server. 

**Parts needed:**\
Jumper wires, (a good assortment of M-F, M-M, and F-F)\
Soldering iron\
Solder wire\
Arduino Nano\
Arduino Mega 2560 or Uno (not Nano, which has too less power for main transciever)\
GPS GT-U7 NEO-6M module\
2 RAYAX LoRa Transciever Module (code: RYLR896 or RYLR890)\
Server module\
iPhone with Prowl firmware installed

**Instructions:**\
Follow the following wiring chart for the reciever. You can use either the 2560 or Uno for the microcontroller.\
|   LoRa   -   2560  |\
|   VDD    -   3V3   |\
|RXD -  4.7KR -  ~2  |\
|  TXD     -    ~3   |\
|  GND     -    GND  |\
[10 K resistor from RXD jumper - GND]\

Follow the following wiring chart for the tracker. \
Upload _reciever.ino_ to the reciever.\
Upload _tracker.ino_ to the tracker.\
Make sure to connect your server to the reciever so it will upload properly.\
Download Prowl on your Iphone to get notifications of location.

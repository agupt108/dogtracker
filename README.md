
 Most dog trackers are really expensive + a subscription if gps tech. The cheaper non subscription modules are bluetooth, limiting their range to around 300 m. However, using **LoRa**, and **Arduino**, we can create a relatively inexpensive GPS tracker that sends location data to a server, processing it and sending it to a phone as a IOS push notifications. LoRa, or Long Range Radio, is a long range wireless data transfer technique that communicates up to 10-15 km on a standard model. Higher end models can communicate up to 716 km. The **RYLR890/96**(either is good) module by Reyax is a very good for this project, because it has a good range of 10-15 km. Two are neeed to make a wireless data transfer, in this case between a dog tracker module and a main module. The data that we will be transferring is the dog's location, which will be found using a GPS module (in this case **GPS Neo-6M, GT-U7, around $12.97 from Amazon**). This data will be send through the LoRa module to the LoRa reciever which will upload the data on the server. 

**Parts needed:**\
Jumper wires\
Soldering iron\
Solder wire\
2 Arduino Nano (you can use 1 2560 or R3 too, but use Nano for the transmitter)\
GPS NEO-6M module\
2 RAYAX LoRa Transciever Module (code: RYLR896 or RYLR890)\
Server module\
iPhone with Prowl firmware installed

**Instructions:**\
Follow the following wiring chart for the reciever.\
\
![reciever](https://user-images.githubusercontent.com/94206551/196574350-b73c118d-97c6-4562-8215-b531f57c456f.png)
\
Follow the following wiring chart for the transmitter. \
![transmitter](https://user-images.githubusercontent.com/94206551/196829894-0d3ffceb-9c47-4e91-9132-0d1da23e8bca.png)

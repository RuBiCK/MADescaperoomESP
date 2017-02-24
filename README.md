# MADescaperoomESP
Arduino program for trigger GPIO ports of ESP8266 from NODE-RED with MQTT

This is an arduino program to be loaded in a ESP8266 that triggers GPIO ports. The trigger is made by NODE-RED inyecting payload in MQTT broker.

This is a WIP project that has started with the examples of OTA and WifiManager

## Main Features
### OTA
As this small chips can be in places with a limited access it's important the ability to reprogram them without physical contact. 
For this feature ESP8266 with 4MB it's needed. I'm using wemos D1 r2

### Captative Portal
We are going to have a bunch of ESPs so it's important an easy way of configuration without any IDE (after first programmin) so I dediced to use WifiManager to create a captative portal and configure the Wifi Credentials aswell the MQTT server and the topic it will be listen. 

### MQTT subscriber
ESP8266 will be listenting a topic and will be notified about when trigger a certain GPIO

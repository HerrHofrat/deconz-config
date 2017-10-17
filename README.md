### deCONZ configuration tool ###

This small tool helps to integrate new sensors to the zigbee network and to rename them.

### Setup ###

Copy the folder to your home assistant installation  `config/www/deconz-config`. It is available at http://<your-hass>/local/deconz-config/index.html  
Enter the deCONZ IP Address and Port or simply click on discover. This will try to get the values from https://dresden-light.appspot.com/discover.  
After that enter the API key and click on open - the config data will be read and a websocket will be opened to get updates from the deCONZ API.  
`Permit join` opens the network for 60 seconds to add new sensors. When a new one is found, a toast message will be displayed and it will be added to the drop-down menu.  
After a sensor is selected, some meta data for this sensor is display - including the current status and the time of the last update. This values are automatically refreshed, once the status has changed.  

### Network functions ###
- permit join for 60 seconds

### Sensor functions ###
- update sensor name
- update sensor configuration
- delete sensor from network

### Known issues  ###
- Currently only works over http
- I only have Xiaomi Door Sensors at the moment - but I assume it will work with any type of sensor.

### Tested devices ###
- Xiaomi Aqara Window Door Sensor
- Xiaomi Aqara Smart Wireless Switch
- Xiaomi Aqara Human Body Sensor

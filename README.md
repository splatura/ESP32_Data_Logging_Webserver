# ESP32_Data_Logging_Webserver
An ESP32/ESP8266 and SHT30 that together form a data logger that is accessed via a webserver and data is graphed via google Charts.

Put both files (ESP32_SHT30_SPIFFS_DataLogger_01.ino and credentials.h) in your sketch folder and modifiy the Wi-Fi access requirements (password and SSID) to match yours via the file tab in the IDE.

Monitor the Serial Port for the assigned IP address and connect to the server with http://IP/ e.g. http://192.168.0.5/

# INA219 data logger branch
Based upon the fantastic work by G6EJD (https://github.com/G6EJD/ESP32_Data_Logging_Webserver), the fork is using the INA219 and the ESP32 to create a voltage/mA tracker.  My purpose for building this is to monitor incoming solar voltage/mA of small solar cells (for 1S LiPo charging) as well as monitoring the power usage of small electronics projects.

This version also adds the ability to update the firmware through the web interface, especially useful when your ESP32 is deployed in a hard to reach place.  It still utilises the ability to be accessed via a webserver and data is graphed via Google Charts.  Check it out at https://github.com/splatura/ESP32_Data_Logging_Webserver/tree/INA219-Data-Logger.

Put all files (ESP32_Data_Logging_Webserver.ino, credentials.h and web.h) in your sketch folder and modifiy the Wi-Fi access requirements (password, SSID and hostname) to match yours via the file tab in the IDE.

Monitor the Serial Port for the assigned IP address and connect to the server with http://IP/ (e.g. http://192.168.0.5/) or http://esp32_logger/

Happy making!


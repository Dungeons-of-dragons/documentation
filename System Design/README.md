# System Design
![alt system design](https://github.com/Dungeons-of-dragons/documentation/blob/main/System%20Design/Home%20system%20design.drawio.png)
The flowchart represents our system design. It is composed of: 
    - Microcontroller(ESP32)
    - Raspberry Pi (model 4B)
    - Application
    - Sensors

The network topology used is the star topology, where all nodes are connected to a central hub using a communication link, that is WiFi in our case.
The communication protocol used is MQTT with the Raspberry Pi as the MQTT broker and the microcontroller and phone as the clients subscribed to it.
The microcontroller is both the Central Control Unit and the Remote Control Unit as it directly receives data from the sensors and gives commands to carry out specific actions.
All data from the microcontroller is stored in a database and the information can be accessed by the user through a mobile application.
The mobile application also acts as an Input Control Unit where the user can manually adjust appliances used in their household.

# Firmware Design
![alt firmware design](https://github.com/Dungeons-of-dragons/documentation/blob/main/System%20Design/home%20firmware.drawio.png)
The flowchart represents our firmware design.
This flow of processes ensures security in users' homes and access to the information present, ready data visualization in their smartphones, analytics of specific data such as energy used in the home, and enabling the user to make changes in to their home appliances.

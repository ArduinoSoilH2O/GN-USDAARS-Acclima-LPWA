# LPWA SIM7070G Gateway

Hardware and firmware for the gateway portion of the node-gateway system.  The gateway is the system master and is responsible for 
synchronizing logged data from the node units (through LoRa radio), storing that data on a local SD card, and pushing that data to 
a server via modem. 

-----------
**NOTE: Users must edit HardwareSerial.h to use configuration strings longer than 64 characters**

HardwareSerial.h is in a path similar to: C:\Program Files (x86)\Arduino\hardware\arduino\avr\cores\arduino\HardwareSerial.h

Change:
#define SERIAL_TX_BUFFER_SIZE 64 to #define SERIAL_TX_BUFFER_SIZE 256

and

#define SERIAL_RX_BUFFER_SIZE 64 to #define SERIAL_RX_BUFFER_SIZE 256

>> To give yourself permission to edit the file, right click on the filename, go to **Properties > Security > Edit...** and give Users "Full control" of the file. You may need Administrator privileges too.

-----------

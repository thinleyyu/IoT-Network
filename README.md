<h1>IoT Network-</h1>
<h2>Raspberry Pi and Teensy-Based Automated Irrigation System with MQTT and Bluetooth</h2>

 ### [YouTube Demonstration](https://youtu.be/NgmdnWOPheM)

<h2>Description</h2>
This project aims to automate water flow management in irrigation channels using a Raspberry Pi, a Teensy microcontroller, and an MQTT broker hosted on AWS. The system monitors water levels and environmental conditions, automates gate controls, and provides real-time data feedback. The setup is particularly suited for remote or rural agricultural applications where reliable water distribution is essential.
<br />


<h3>Languages</h3>
- <b>Python: Used on the Raspberry Pi for writing MQTT clients (publisher and subscriber) to communicate with the MQTT broker on AWS, as well as handling Bluetooth communication.</b> 
- <b>C++ (Arduino): Used to program the Teensy microcontroller for sensor readings, servo control, and Bluetooth data transmission.</b>

<h3>Utilities and Libraries</h3>

- <b>paho-mqtt (Python): A Python MQTT library used on the Raspberry Pi to connect to the MQTT broker on AWS, publish sensor data, and receive control messages.</b>
- <b>PySerial (Python): Used to handle serial communication over Bluetooth between the Raspberry Pi and Teensy.</b>
- <b>DHT (Arduino): An Arduino library used to interface with the DHT11 sensor for temperature and humidity readings.</b>
- <b>Servo (Arduino): Standard Arduino library to control the SG90 servo motors connected to the Teensy.</b>
- <b>Mosquitto MQTT Broker: Installed and configured on AWS EC2 for secure MQTT communication with Transport Layer Security (TLS).</b>
- <b>AWS IoT Core: Manages MQTT broker setup and TLS certificate generation for secure communication.</b>
- <b>OpenSSL: Used to generate and manage TLS certificates for secure communication with the MQTT broker on AWS.</b> 


<h2>Environments Used </h2>

- <b> AWS EC2: Amazon Linux 2 (Kernel 4.14)
Purpose: Hosts the Mosquitto MQTT broker for secure communication between devices. Configured with Transport Layer Security (TLS) for encrypted data transfer. </b> 
- <b> Raspberry Pi: Raspberry Pi OS (Debian-based, 32-bit, Kernel 5.10)
Purpose: Serves as the main control system, handling data from the Teensy over Bluetooth and managing MQTT communication with AWS. </b> 
- <b> Teensy Microcontroller: Arduino-like Environment
Purpose: Collects sensor data (water level, temperature, and humidity) and manages servo motors and LEDs. Communicates with Raspberry Pi over Bluetooth </b> 
- <b> Local Development (MacBook): macOS Ventura (13.0)
Purpose: Used for project setup, configuring remote connections, transferring files, and debugging. </b> 
<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

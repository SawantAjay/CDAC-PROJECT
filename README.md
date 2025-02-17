# Project Description: Fire and Hazard Detection for buildings using CAN and IoT

#Overview
This project focuses on developing a Fire and Hazard Detection System using Controller Area Network (CAN) and IoT. The system consists of two nodes:
Transmitter Node – Monitors environmental conditions using sensors and transmits data via CAN.
Receiver Node – Receives the sensor data, triggers alerts when hazards are detected, and uploads the data to the Blynk cloud for remote monitoring.

#Hardware Components
ESP32 – Microcontroller for data processing and communication.
MCP2515 CAN Transceiver – Handles CAN communication between nodes.
MQ-2 Gas Sensor – Detects hazardous gas leaks.
DHT11 Sensor – Monitors temperature and humidity.
Flame Sensor – Detects fire or flames.
Buzzer – Provides audible alerts in case of a hazard.
I2C LCD Display – Displays real-time data and alerts.


#Working Principle

1) Transmitter Node (Sensor Data Collection & Transmission) -:
Reads sensor data from MQ-2, DHT11, and the flame sensor.
If gas concentration exceeds a threshold, fire is detected, or temperature is too high, an alert is triggered.
Transmits the sensor data to the receiver node via CAN communication.

2) Receiver Node (Alert & IoT Integration) -:
Receives the data from the transmitter node using MCP2515.
If any hazard (fire, gas leak, or high temperature) is detected:
The buzzer starts beeping as an immediate alert.
The warning message is displayed on the LCD screen.
The data is uploaded to the Blynk cloud, making it accessible remotely.
An alert notification is sent to the Blynk app and an email is triggered for immediate user awareness.


#Features & Functionalities
✅ Real-time Monitoring – Continuously tracks fire, gas leakage, temperature, and humidity.
✅ Wireless Alerts – Sends instant notifications via Blynk app and email.
✅ Audible Alarm – Activates a buzzer for on-site alerting.
✅ CAN Communication – Ensures reliable and fast data exchange between nodes.
✅ LCD Display – Provides real-time data and warning messages.
✅ IoT Integration – Enables remote monitoring through Blynk.

#Applications
🔥 Industrial Safety – Prevents fire and gas hazards in factories and plants.
🏠 Home & Building Automation – Enhances safety in homes and commercial buildings.
🚗 Automotive Safety – Can be adapted for vehicle fire detection systems.

This system ensures real-time hazard detection and immediate alerts, making it an effective safety solution for various applications. 🚀🔥

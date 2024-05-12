This is a repository created to document our final microprocessor class project.

# Industry Fault Detection IOT System (IDFS)

## Overview

The Industry Fault Detection System (IDFS) is am autonomous monitoring solution designed to detect and prevent potential failures in industrial settings. Leveraging IoT technologies and real-time data analytics, IDFS continuously monitors critical parameters, identifies anomalies, and takes proactive measures to mitigate risks. This system enhances operational efficiency, reduces downtime, and ensures a safer working environment.

## Features

### Detection
- **Light Failures:** Monitors illumination levels to ensure adequate lighting in critical areas, preventing hazards associated with poor visibility.
- **Heat and Humidity Levels:** Tracks temperature and humidity to prevent overheating, mold growth, and occupant discomfort.
- **Harmful Gases:** Detects the presence of dangerous gases, enabling prompt corrective actions to maintain air quality and safety.
- **Flood Detection:** Identifies potential water leaks or flooding, allowing for quick response to prevent extensive water damage.
-**Flame Detection:** Detects fire on plant.

### Auxiliary Systems
- **Gas Detection Extraction Fan:** Quickly removes harmful gases from the environment, ensuring a healthier atmosphere.
- **Sprinkler System Water Pump:** Ensures water availability for fire suppression, enhancing safety and minimizing damage.
- **IoT Monitoring:** Real-time data collection and analysis optimize operations and improve response times.

## Materials
- **Air Quality Sensor (MQ-135):** Detects a wide range of gases with high sensitivity and fast response.
- **Light Detection Sensor (LDR):** Senses light conditions, used with microcontrollers for easy integration.
- **Infrared Water Level Sensor:** Measures liquid levels accurately with no moving parts.
- **Infrared Flame Detector:** Detects fire presence with high reliability and precision.
- **Temperature and Humidity Sensor (DHT11):** Measures temperature and humidity with high accuracy.

## Methodology
The system uses various sensors to detect industrial faults:
- **Gas Detection:** Measures gas concentration and activates a fan if levels are unsafe.
- **Infrared Light Sensor:** Detects combustion.
- **Water/Flood Level Sensor:** Monitors water presence and alerts on detection.
- **Light Detection:** Monitors electrical lighting circuit faults.
- **Temperature and Humidity Sensor:** Controls environmental conditions to prevent hazards.

Sensors are connected to an Arduino Mega, with a master-slave configuration to the Nano 33 IOT for remote monitoring via Blynk. The system uploads data to the cloud for future reports and instant notifications.

## Circuit Design
The circuit design integrates all mentioned sensors using Fritzing. Unavailable sensors in Fritzing were simulated with other components.

## Prototype
Initial issues included establishing a stable connection between the Nano 33 IOT and Blynk, data transfer between the Mega and Nano, and power supply complications. These were resolved by code modifications and adding a 5V 1A power supply, resulting in a reliable and efficient system.

## Future Work
Future enhancements will focus on:
- **Independence from Plant Power:** Incorporate dedicated power sources like solar panels or backup batteries.
- **Local Monitoring Subsystem:** Allow on-site personnel to access real-time data and alerts.
- **Custom PCB Design:** Simplify the system by consolidating components into a single, compact unit, enhancing robustness and accessibility.

## Conclusion
Our project successfully developed an autonomous Industry Fault Detection System that integrates IoT technologies and real-time data analytics. Overcoming initial challenges, the IDFS now reliably monitors industrial parameters, detects faults, and takes proactive measures to enhance operational efficiency and safety. This project demonstrates the potential for creating smarter, more responsive, and safer industrial environments.

## Repository Structure
- In "Codes_Libraries_IFDS" you can find the codes for Arduino Mega (Master) and Nano 33 IOT (Slave).
- In the fzz file the  Circuit diagrams and Fritzing files can be found.

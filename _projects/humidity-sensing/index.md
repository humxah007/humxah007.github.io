---
layout: post
title: Humidity and Temperature Sensing
description: A real-time humidity monitoring system using Arduino and DHT11 sensor demonstrating environmental data acquisition and temperature-compensated readings.
skills: 
  - Arduino programming
  - Sensor interfacing
  - Circuit design
  - Environmental monitoring
  - Data processing
  - Real-time display
main-image: /_projects/humidity-sensing/pictures/profile.jpg
---

# Detailed Description
This project focused on designing and implementing a humidity and temperature sensing system using an Arduino microcontroller paired with a DHT11 sensor. The sensor provided both humidity and temperature readings, which were processed in real-time by the Arduino and displayed on a connected screen.

The readings were validated and calibrated to ensure accuracy (within 2–5%), with the system effectively compensating for temperature effects on humidity measurements. The setup highlights the importance of environmental sensing in modern applications and provides a hands-on demonstration of embedded system design and sensor data visualization.

## Analysis
The DHT11 sensor's resistance-based humidity measurement was verified through repeated testing. Calibration steps confirmed consistent output within the expected accuracy range. The system's real-time performance and ease of use make it suitable for small-scale environmental monitoring.

### Conclusion
This project demonstrates the successful use of Arduino and sensor integration for real-time humidity and temperature monitoring. The experiment proves useful in educational, experimental, and basic environmental sensing applications.

## Project Components
{% include image-gallery.html images="/_projects/humidity-sensing/pictures/arduino.jpg, /_projects/humidity-sensing/pictures/sensor.jpg, /_projects/humidity-sensing/pictures/wires.jpg" height="300"%}
<span style="font-size: 10px">Arduino board, DHT11 sensor, and wiring connections</span>  

## Circuit Setup
{% include image-gallery.html images="/_projects/humidity-sensing/pictures/connection.jpg" height="400"%}
<span style="font-size: 10px">Complete circuit diagram and physical implementation</span>  

## Demonstration Video
{% include youtube-video.html id="1AgcNQ-J0Y8" autoplay="false"%}

## Component Specifications

| Component          | Description                               |
|--------------------|-------------------------------------------|
| Arduino Uno        | Microcontroller board for data processing |
| DHT11 Sensor       | Measures temperature and humidity         |
| LCD/Serial Monitor | Displays real-time data                   |
| Jumper Wires       | Connections between components            |
| Breadboard         | Prototyping platform                      |

> "Knowing your environment is the first step to controlling it."

## Additional Notes
Future versions could include wireless data logging and integration with cloud-based platforms for remote environmental tracking.

**External Resources:**  
[Arduino DHT11 Library Documentation](https://www.arduino.cc/reference/en/libraries/dht-sensor-library/)

# Complete Smart Home System with Enhanced Safety Features

IoT smart-home graduation project with embedded safety modules, PCB design, MQTT communication, Python server, database, Flutter mobile app and custom mechanical designs.

It was designed for home automation and safety-oriented monitoring for fire, flooding, motion, door opening, temperature, alarms, electrical loads, and power availability.

> The original implementation used a MQTT broker locally configured, a Python server, a database and hardware modules based on ESP8266. To reproduce live functionality, the local environment must be rebuilt and configured.

## Project resources

- [Android application release](../../releases/latest)
- [Mechanical designs on GrabCAD](https://grabcad.com/library/complete-smart-home-system-with-enhanced-safety-features-1)
- [Final project report](https://drive.google.com/file/d/1AwJD1UMMyeOQV9r7DHtg-fEgsQMXAIIb/view?usp=sharing)
- [Academic poster](https://drive.google.com/file/d/1HJPEl7pNxOwpySByrP_OhR2CXyU3-c1F/view?usp=sharing)
- [Final presentation](https://drive.google.com/file/d/1ijiyFpCKpJ4Y58pfwwHIocHStm_BWEi7/view?usp=sharing)

## System overview

The project is based on ESP8266 modules connected over a local network. MQTT allows messages exchange between hardware, Python server and mobile application. The server interfaces with the database of the project.

<p align="center">
  <a href="docs/project-overview/All%20in%20One%20Schematic.jpg">
    <img src="docs/project-overview/All%20in%20One%20Schematic%20Preview.jpg"
         alt="Complete smart-home system schematic"
         width="900">
  </a>
</p>

<p align="center">
  <em>Click the preview to open the full-resolution system schematic.</em>
</p>

## Main modules

The system was organized into ten functional modules:

1. **Dual Channel Relay** — control of two connected electrical loads.
2. **UPS** — backup power.
3. **Fire Detection Module** — fire hazard detection.
4. **IR Transceiver Module** — infrared control of compatible appliances.
5. **Motion Detection Module** — motion monitoring.
6. **Alarm Module** — audible alarm control.
7. **Temperature Module** — environmental temperature monitoring.
8. **Flood Detection Module** — water and flooding detection.
9. **Door Opening Detection Module** — door-opening monitoring.
10. **Power Meter Module** — electrical power-monitoring interface.

### Firmware availability

Firmware source code is only provided for **Alarm Module** and **Flood Detection Module** as a sample of representative implementations. The original firmware of the other eight modules is not found in the archived project files.

The two examples included are not the full firmware needed to run the full ten-module system.

## Mobile application

The Android app was developed using Flutter. It gives interfaces to configure the server, to communicate with MQTT, to control modules, to send notifications, and to change system settings.

Android build is available from the [latest GitHub Release](../../releases/latest).

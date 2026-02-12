# Goal of the project
My goal with this project is to
- Learn about working with IoT devices and Microservers
- Learn about the DevOps patterns and solutions with the technologies involved.
- Make a useful, dependable, reliable and fun application.

## Project state
- In planning
- Waiting for Parts (Arduino)

# Surveillance-pipeline-prototype
A project for prototyping a C++ based devOps stack

Goal of this project is to build a surveillance system prototype to be a basis for derivative projects in the future. Idea of this project is to follow live sensor data with an IoT device, that when meeting set circumstances reports to central microserver. Microserver should complete set tasks when alerted by the IoT device.

## System usecases
Any quiet waiting for an event that could happen, and what should be detected, recorded and/or reacted to.

### Usecases from ordinary life:
- Camera surveillance within limits of private property: IoT-device detects sound of steps nearby with its integrated machine learning model and alerts the Microserver: "Steps detected!". Microserver then forwards the message with e.g. ntfy.sh to administrator's phone and starts recording with attached camera.

- IoT-device detects a condition like unexpected temperature drop. Similar path to the previous example is used to report. Such report can be vital in avoiding unwanted consequences, like house water pipes freezing at winter because the automatic door of the garage within the house was found to have been somehow opened.

- Can be adatped to various different scenarios and circumstances, to monitor activity happening on desired sounds or patterns.

# Details
### Planned IoT device: Arduino Nano 33 Sense BLE
- Continuous power or powerbank (re-charge within 1-2weeks)
- Can be set to sleep until triggered by an event (harder to detect)
- Allows sound and movement analytics, light and temperature level tracking

### Planned Microserver: Raspberry Pi 4 4GB
- Requires dependable continuous 5V/3A power
- Has wide possibilities for reaction actions, like
    - Attached camera
    - Sending message/alert via some channel (internet)
    - Forwarding and/or collecting IoT-transmitted data (internet, local database)

Planned connection between used devices: BLE
In this prototype project the Raspbery Pi is connected to interned by wire.






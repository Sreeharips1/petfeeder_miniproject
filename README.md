Project Overview

Our project addresses the challenge of caring for pets when the family is away due to work or vacations. Feeding and providing water for pets in such situations can be difficult, and to solve this problem, we developed a smart pet feeding and monitoring system.

With the simple press of a button on a smartphone, users can:

Dispense food and water for their pets remotely.
Monitor their pet in real-time via a camera feed.
Receive notifications when food or water is dispensed and when the pet consumes them.
Ensure proper waste management by automatically clearing leftover food into a waste bin.
Monitor the levels of food and water in the dispensers using ultrasonic sensors.
Key Features
Remote Food and Water Dispensing:

Operated via the Blynk mobile application.
Notifications sent via Telegram for every action performed.
Real-Time Monitoring:

An ESP CAM module provides live video feeds of the pet, allowing users to monitor their activity.
Automated Notifications:

A load cell sensor detects when food or water is dispensed and consumed, triggering a Telegram notification.
Food Waste Management:

A servo motor rotates the food bowl to dispose of leftovers into a waste bin automatically.
Tank Level Monitoring:

Ultrasonic sensors measure food and water levels in the dispensers, ensuring timely refilling.
Components and Their Roles
ESP Microcontrollers (2 Units):

ESP #1: Handles the food dispenser and related notifications.
ESP #2: Controls the water dispenser and related notifications.
Servo Motors (3 Units):

2 Servos: Control the opening mechanisms of the food and water dispensers.
1 Servo: Rotates the food bowl to dispose of leftover food into a waste bin.
Load Cell and HX711 Amplifier:

Measures the weight of food and water dispensed into the bowl.
Sends data to the ESP module to trigger Telegram notifications:
When food or water is dispensed.
When the pet consumes food or water.
Ultrasonic Sensors:

Mounted above the food and water dispensers to measure and monitor the levels of food and water.
ESP CAM Module:

Streams a live video feed of the pet directly to the user's smartphone.
Blynk Mobile Application:

Provides an interface for controlling all functionalities, including dispensing food and water, monitoring levels, and activating the waste management system.
Working Mechanism
Food and Water Dispensing:

A command sent from the Blynk app triggers the respective ESP module.
The ESP signals the corresponding servo motor to open the food or water dispenser.
Food or water is released into the bowl, and the load cell measures the dispensed amount.
The ESP sends a notification to the user's phone via Telegram indicating the action.
Consumption Notification:

When the pet consumes food or water, the load cell detects a weight change and sends this data to the ESP.
A notification, such as "Pet has eaten" or "Pet has drunk water," is sent to the user.
Waste Management:

A separate servo motor rotates the bowl after a predefined interval or on user command, dumping leftovers into the waste bin below.
Monitoring:

The ESP CAM streams live video to the user’s phone, enabling real-time monitoring of the pet.
Level Monitoring:

Ultrasonic sensors continuously measure the food and water levels in the dispensers.
When levels are low, notifications are sent via Telegram to prompt a refill.
Data Communication:

The ESP modules communicate with the sensors and actuators using GPIO pins.
All signals are processed by the ESP modules and transmitted to the mobile app and Telegram using Wi-Fi.
Highlights for Interview
Innovation: Provides a comprehensive solution to pet care with automation, monitoring, and waste management.
Technologies Used: IoT-enabled components (ESP modules, sensors, and mobile app integration).
Scalability: Can be enhanced with AI to track pet behavior or add voice commands for control.
Practical Applications: Ideal for pet owners who frequently travel or work long hours.
This project demonstrates proficiency in IoT, embedded systems, and mobile app integration. It showcases how everyday challenges can be solved with technology and automation.

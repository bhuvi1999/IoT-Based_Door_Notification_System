# IoT-Based Door Notification System
## Project Overview
This repository contains the code and documentation for an IoT-Based Door Notification System built using the ESP8266 NodeMCU and integrated with IFTTT (If This Then That) to provide real-time door state monitoring. The system detects door open/close events using a magnetic switch sensor and sends instant notifications to the user’s phone via Wi-Fi. This project demonstrates practical IoT applications for home security and remote monitoring.

## Project Features
- **Real-Time Monitoring:** Utilizes a magnetic switch sensor to detect door state changes (open/close).
- **Instant Notifications:** Triggers IFTTT applets to push notifications to the user’s phone when the door state changes.
- **Electronic Circuit Logic:** A break in magnetic contact activates a Wi-Fi signal to notify users, ensuring reliable detection.
- **Lightweight Design:** Built with the ESP8266 NodeMCU for efficient, low-cost IoT implementation.

## Tools and Technologies
### Hardware:
1. ESP8266 NodeMCU
2. Magnetic Switch Sensor
### Software:
1. Arduino IDE (for programming the ESP8266)
2. IFTTT (for configuring notification applets)
### Protocols: Wi-Fi (for communication between ESP8266 and IFTTT)

## How It Works
1. The magnetic switch sensor is connected to the ESP8266 NodeMCU, monitoring the door’s state.
2. When the door opens or closes, the magnetic contact breaks, generating a signal.
3. The ESP8266 detects this signal and sends a request to an **IFTTT webhook** over Wi-Fi.
4. The IFTTT applet triggers a notification to the user’s phone, alerting them to the door state change.

## Repository Structure
- **/src:** Contains the Arduino sketch (door_notification.ino) for programming the ESP8266.
- **/docs:** Includes documentation, such as circuit diagrams, setup guides, and IFTTT configuration steps.
- **/examples:** Provides sample code snippets for testing sensor and Wi-Fi connectivity.
- **README.md:** This file, detailing the project overview and setup.

## Setup Instructions
1. *Hardware Setup:*
  - Connect the magnetic switch sensor to the ESP8266 NodeMCU (e.g., to a digital pin like D1 and GND).
  - Ensure the NodeMCU is powered via USB or an external power source.
2. *Software Setup:*
  - Install the Arduino IDE and add ESP8266 board support (via Board Manager).
  - Install required libraries **(e.g., ESP8266WiFi, ESP8266HTTPClient)**.
  - Configure Wi-Fi credentials and IFTTT webhook key in the Arduino sketch.
3. *IFTTT Configuration:*
  - Create an IFTTT applet with a Webhooks trigger and a notification action.
  - Copy the webhook URL and integrate it into the Arduino code.
4. *Upload Code:*
  - Upload the door_notification.ino sketch to the **NodeMCU** using the **Arduino IDE**.
5. *Test:*
  - Open/close the door to verify that notifications are sent to your phone.

## Key Takeaways

This project showcases my ability to design and implement an IoT-based solution for real-time monitoring, integrating hardware (ESP8266, magnetic switch) with cloud services (IFTTT). It demonstrates skills in embedded programming, circuit design, and IoT communication protocols, applicable to smart home and security systems.

Contact

For questions or collaboration opportunities, reach out via LinkedIn or email.

# BuildFest-2.0
Representing our prototype bot : ProtoPulse Rover meant for supplying emergency supplies to areas where humans cant reach due to any mishappening.


# ProtoPulse — Emergency Supply Rover 🤖

**An ESP32-based robotic rover designed to transport emergency supplies while detecting and avoiding obstacles.**

Developed by **Team ProtoPulse**  
**Team Members:** Yovin Kumar and Vaibhav Arora  
**Institution:** Guru Nanak Dev University (GNDU), Amritsar  
**Project:** PS-26 — Emergency Supply Rover

---

## 📌 Project Overview

The Emergency Supply Rover is a prototype designed to transport essential supplies, such as first-aid kits, medicines, and other lightweight emergency packages, to designated locations.

The robot uses an ESP32 microcontroller for control, an ultrasonic sensor for obstacle detection, and DC gear motors for movement. Its obstacle-avoidance mechanism allows it to detect objects in its path and change direction to navigate around them.

The project aims to demonstrate a low-cost, practical robotic solution for emergency supply transportation.

## 🎯 Objectives

- Develop a working emergency supply transportation rover.
- Achieve a minimum payload capacity of **1 kg**.
- Detect and avoid obstacles autonomously.
- Implement reliable motor control and navigation.
- Develop a smartphone-based dashboard for monitoring and controlling the rover.
- Explore camera integration for visual monitoring.

## ⚙️ Hardware Components

| Component | Purpose |
|---|---|
| ESP32 Development Board | Main controller and processing unit |
| L298N Motor Driver | Controls the DC gear motors |
| DC Gear Motors (without encoders) | Provides locomotion |
| HC-SR04 Ultrasonic Sensor | Measures distance to obstacles |
| SG90 Servo Motor | Rotates the ultrasonic sensor for directional scanning |
| Wheels and Chassis | Mechanical structure and movement |
| 18650 Battery Pack | Power supply |

*The component list describes the current prototype; additional components may be incorporated during development.*

## 🚀 Current Features

- **Obstacle Detection:** Measures the distance to objects using an ultrasonic sensor.
- **Automatic Obstacle Avoidance:** Stops when an obstacle is detected within a defined distance and scans for an alternative direction.
- **Motor Control:** Supports forward, backward, left, right, and stop operations.
- **Payload Transportation:** Carries emergency supplies and additional test loads.
- **Expandable Architecture:** Designed to support future wireless monitoring and camera integration.

## 🧪 Payload Testing and Results

The project requirements specified that the rover should be capable of carrying a **1 kg payload**.

During our testing, we experimented with an additional external load of approximately **1–1.5 kg**. The rover was able to carry the load and move smoothly during these tests.

These results indicate that the prototype can handle the required payload under the tested conditions. Further systematic testing would be needed to establish its maximum safe payload capacity and endurance.

## ⚠️ Current Limitation: Motor RPM Variation

The rover currently tends to follow a **curved path instead of moving perfectly straight**, even when both motors have the same rated specifications.

This occurs because the two motors may rotate at slightly different actual RPMs under the same input. Manufacturing tolerances, gearbox friction, wheel differences, and load distribution can contribute to this variation.

### Proposed Improvement

The planned solution is to use **encoder-equipped motors** with closed-loop speed control.

Wheel encoders can measure the actual rotational speed of each motor, allowing the controller to adjust their speeds independently and improve straight-line movement.

For the current prototype, non-encoder gear motors are being used, so precise wheel-speed feedback and correction are not yet available.

## 📱 Smartphone Dashboard — In Development

A phone-based dashboard is currently being developed and is targeted for completion by **Day 3 of the project event**.

Planned functionality includes:

- Displaying rover status and operating state.
- Monitoring obstacle distance.
- Providing remote movement controls.
- Displaying alerts and relevant navigation information.
- Supporting an emergency-stop command.

The dashboard is a work in progress and should not be considered a completed feature until integration and testing are finished.

## 📷 Planned Camera Integration

Camera integration is also planned to provide a visual view from the rover.

The intended functionality is to enable remote visual monitoring and help the operator observe the rover's surroundings.

Live camera streaming, its integration with the phone dashboard, and reliable operation will require further implementation and testing.

## 🔧 Future Improvements

- Integrate encoder-equipped motors for improved straight-line navigation.
- Implement closed-loop motor speed control.
- Complete and test the smartphone dashboard.
- Integrate live camera streaming.
- Improve navigation reliability across different surfaces.
- Conduct repeatable payload, obstacle-avoidance, and battery-endurance tests.
- Explore GPS or waypoint-based navigation for suitable outdoor applications.

## 🏁 Conclusion

ProtoPulse's Emergency Supply Rover demonstrates a working approach to low-cost robotic transportation of emergency supplies. The prototype has demonstrated obstacle detection and avoidance, movement control, and successful transportation of a test load exceeding the specified 1 kg requirement under the conditions tested.

With improvements in motor feedback, remote monitoring, and camera integration, the platform can be developed into a more capable and reliable emergency-response robotics system.

---

**Built with curiosity, electronics, and robotics by Team ProtoPulse.** 🤖

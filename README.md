
# Autonomous Robotic Vehicle Using Raspberry Pi  

Welcome to the repository for the **Autonomous Robotic Vehicle Using Raspberry Pi**! This project demonstrates the development of a vision-based autonomous robotic vehicle capable of lane detection and navigation in a controlled environment. It serves as the first phase of a multi-stage project aimed at building a fully autonomous navigation system.  

---

## Table of Contents  
1. [Introduction](#introduction)  
2. [Features](#features)  
3. [Hardware Requirements](#hardware-requirements)  
4. [Software Requirements](#software-requirements)  
5. [System Overview](#system-overview)  
6. [Implementation Details](#implementation-details)  
   - [Lane Detection](#lane-detection)  
   - [Obstacle Avoidance](#obstacle-avoidance)  
   - [Motion Control](#motion-control)  
7. [Results](#results)  
8. [Future Enhancements](#future-enhancements)  
9. [How to Use](#how-to-use)  
10. [Contributors](#contributors)  

---

## Introduction  
This project involves the design and implementation of an autonomous robotic vehicle that uses computer vision and sensor integration to navigate a predefined path. The system employs a Raspberry Pi for processing, a Pi Camera for vision-based lane detection, and ultrasonic sensors for obstacle avoidance.  

---

## Features  
- **Lane Detection**: Uses computer vision techniques like Gaussian Blur, Canny Edge Detection, and Hough Transform to identify lane boundaries.  
- **Obstacle Detection and Avoidance**: Utilizes ultrasonic sensors to dynamically adjust the path and prevent collisions.  
- **Real-Time Navigation**: Processes data in real time to ensure smooth and stable motion.  
- **Hardware Integration**: Combines Raspberry Pi, motor drivers, and sensors into a cohesive system.  

---

## Hardware Requirements  
- **Raspberry Pi 4 Model B** (2GB/4GB/8GB RAM)  
- **Pi Camera Module 2**  
- **L298N Motor Driver**  
- **HC-SR04 Ultrasonic Sensors**  
- **3.7V Lithium-Ion Battery Pack**  
- **Four-Wheel Robotic Chassis**  
- **SG90 Servo Motor**  

---

## Software Requirements  
- **Python 3.7+**  
- **OpenCV Library**  
- **RPi.GPIO Library**  
- **Picamera2 Library**  

---

## System Overview  
The system consists of:  
- **Camera Module**: Captures real-time video for vision-based navigation.  
- **Raspberry Pi**: Processes video and sensor data, runs decision-making algorithms.  
- **Ultrasonic Sensors**: Detect obstacles and measure distances.  
- **Motor Driver and Motors**: Control movement and ensure smooth navigation.  

### Workflow:  
1. Capture live video using the Pi Camera.  
2. Process the video feed to detect lanes.  
3. Use sensor data to adjust the vehicle’s path dynamically.  
4. Control motors to follow the lane and avoid obstacles.  

---

## Implementation Details  

### Lane Detection  
- **Gaussian Blur**: Reduces noise for better edge detection.  
- **Canny Edge Detection**: Identifies edges in the image.  
- **Hough Transform**: Detects straight lines representing lane boundaries.  

### Obstacle Avoidance  
- **HC-SR04 sensors** measure the distance to obstacles.  
- The **Raspberry Pi** adjusts the vehicle’s trajectory based on sensor feedback.  

### Motion Control  
- **L298N Motor Driver** regulates the speed and direction of DC motors.  
- **PWM signals** control the motors for precise movement.  

---

## Results  
- Successfully detected and followed lanes in real-time.  
- Demonstrated dynamic obstacle avoidance.  
- Achieved stable and reliable navigation under controlled conditions.  

---

## Future Enhancements  
- Implement machine learning for adaptive lane detection.  
- Add feedback mechanisms like encoders for better motor control.  
- Enhance the system to handle real-world challenges like broken lanes, shadows, and glare.  
- Integrate dynamic path planning for complex environments.  

---

## How to Use  

1. **Clone the Repository**:  
   ```bash  
   git clone https://github.com/<your-username>/<repository-name>.git  
   ```  

2. **Set up the Hardware**:  
   Follow the instructions in the documentation to assemble the hardware components.  

3. **Install the Required Libraries**:  
   Run the following command to install dependencies:  
   ```bash  
   pip install opencv-python RPi.GPIO picamera2  
   ```  

4. **Run the Main Script**:  
   Execute the main script to start the autonomous navigation system:  
   ```bash  
   python main.py  
   ```  

5. **Observe**:  
   Watch the vehicle as it navigates the path and avoids obstacles in real time.  

---

## Contributors  
- **Sachin**  
- **Ashish Barpete** 
- **Kajal** 
- **Supervisor**: Dr. Soumitra K. Nayak  


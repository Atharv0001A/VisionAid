# VisionAid
Vision Aid is an innovative wearable solution designed to assist visually impaired individuals in navigating their surroundings and performing daily tasks more independently. Developed in the form of smart glasses, the system integrates multiple sensors and technologies to provide real-time assistance through audio feedback and haptic alerts.
Key Features:
1.Obstacle Detection:
Uses an ultrasonic sensor mounted on the glasses to detect nearby obstacles.
When an object is detected within a certain range, the system sends a voice alert through an earphone and activates a vibration motor as haptic feedback.
2.Face Detection:
Incorporates the ESP32-CAM module to recognize human faces.
When a known or unknown face is detected, it notifies the user through voice messages via earphones.
3.Health Monitoring:
Equipped with the MAX30100/30102 sensor to monitor heart rate (BPM) and SpO2 (oxygen saturation).
Vital signs can be recorded and monitored in real-time for user safety.
4.Fall Detection & SOS Alert:
Uses an accelerometer (MPU6050) to detect falls or unusual movements.
When a fall is detected, the system sends an SOS signal to a caretaker using Wi-Fi and ThingSpeak integration.
5.Location Tracking:
Integrated GPS (NEO-6M module) allows tracking of the user’s location.
GPS coordinates can be sent to caretakers in emergency situations.
6.Wireless Communication:
Utilizes Wi-Fi (HTTP or MQTT) or Bluetooth to transmit data from the ESP32 modules to the Raspberry Pi 4, which acts as the central controller and audio output device.
7.Braille Support (Optional Add-On):
Includes a Braille chart representation in the dashboard to help caretakers understand the system better.
Future versions aim to integrate text-to-Braille conversion using solenoids to create a tactile display for blind users.

Technical Components:
Raspberry Pi 4 Model B (4GB),
ESP32 & ESP32-CAM,
MAX30102 (Heart Rate & SpO2 Sensor),
MPU6050 (Accelerometer),
NEO-6M GPS Module,
HC-SR04 (Ultrasonic Sensor),
Vibration Motor,
Earphones for voice output,
Batteries: 3.7V and 12V with voltage converters,

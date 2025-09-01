
# 3-in-1 Smart Car

**Bluetooth Control • Line Following • Obstacle Avoidance**

This project showcases a **multi-functional robotic car** that integrates **three control modes** into a single platform:

1. **Bluetooth Control** – Drive the car manually using a smartphone app or controller.
2. **Line Following** – Automatically follow a track using IR sensors.
3. **Obstacle Avoidance** – Detect and avoid obstacles using ultrasonic sensors.

The car is designed to be versatile, educational, and fun — a great example of combining hardware, sensors, and embedded programming.


<p align="center">
  <img src="1-2.png" width="50%">
  <img src="2-2.png" width="50%">
</p>


---

## 🚗 Features

* **Bluetooth Control**

  * Control direction and speed via mobile app.
  * Smooth forward, backward, left, right movements.

* **Line Following Mode**

  * IR sensors detect black/white tracks.
  * Algorithm adjusts motor speed to stay on track.

* **Obstacle Avoidance Mode**

  * Ultrasonic sensor measures distance.
  * Automatically stops and reroutes around obstacles.

* **Single Hardware Platform**

  * Switch between modes without rewiring.
  * Compact design with minimal components.

---

## 🛠 Hardware Components

* **Microcontroller:** Arduino UNO / Mega (or similar)
* **Motor Driver:** L298N / L293D
* **Motors:** 2x or 4x DC gear motors
* **Sensors:**

  * IR sensors for line following
  * Ultrasonic sensor (HC-SR04) for obstacle avoidance
* **Bluetooth Module:** HC-05 / HC-06
* **Power Supply:** Li-ion battery or AA battery pack
* **Chassis:** 2WD or 4WD acrylic/metal platform

---

## 💻 Software Requirements

* **Arduino IDE** (latest version recommended)
* Required Libraries:

  * `AFMotor.h` (if using Adafruit Motor Shield)
  * `SoftwareSerial.h` (for Bluetooth)

Upload the provided `.ino` file to your Arduino to get started.

---

## ⚡ How It Works

1. **Mode Selection:**

   * A switch or Bluetooth command selects one of three modes.

2. **Bluetooth Mode:**

   * The Arduino listens for commands from the Bluetooth module and adjusts motor speed/direction accordingly.

3. **Line Following Mode:**

   * IR sensors continuously read track position.
   * The Arduino adjusts motor speeds to stay centered on the line.

4. **Obstacle Avoidance Mode:**

   * The ultrasonic sensor measures distance ahead.
   * If an obstacle is detected within a threshold, the car stops and turns automatically.

---


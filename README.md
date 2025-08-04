# SENSI — Assistive Wearable Technology

**SENSI** is an innovative, wearable assistive device designed to support individuals with visual and/or hearing impairments. The MVP (Minimum Viable Product) focuses on real-time environmental awareness through haptic feedback, helping users navigate and respond to their surroundings safely and independently.

---

##  Project Status: MVP (Minimum Viable Product)

This is the first working prototype of SENSI, showcasing core functionalities including:
* Obstacle detection via ultrasonic sensors
* Haptic feedback for proximity alerts
* Basic sound detection and classification (e.g., horns, alarms)
* Bluetooth integration with mobile navigation apps (basic alerts)

---

##  Core Features

| Feature                 | Description                                                                 |
| :---------------------- | :-------------------------------------------------------------------------- |
|  Sound Detection      | Recognizes critical sounds (horns, sirens) and alerts the user via vibration |
|  Obstacle Detection   | Ultrasonic sensors detect nearby objects and trigger warning vibrations     |
|  Mobile Integration   | Pairs with smartphone GPS for directional feedback                          |
|  Custom Feedback Patterns | Vibrations vary by alert type to allow non-verbal recognition               |
|  Power Efficient      | Optimized for low-power operation with rechargeable battery                 |

---

##  Tech Stack

* **Hardware**: Arduino Nano / ESP32, Ultrasonic sensor (HC-SR04), Microphone module, Vibration motor, Bluetooth module (e.g., HC-05), Rechargeable Li-Po battery
* **Software**:
    * Arduino IDE (C++)
    * Optional: Android companion app (Kotlin/Java)
    * Sound classification via basic FFT (Fast Fourier Transform)

---

## 💻 My Contribution

* Designed and assembled the wearable hardware prototype, integrating ultrasonic sensors, microphone, and haptic feedback motors.
* Developed the microcontroller firmware in Arduino IDE (C++) for real-time obstacle and sound detection.
* Implemented custom vibration patterns for distinct alert types to enhance user recognition.
* Conducted initial testing and identified key limitations for future optimization.

---

##  Installation & Setup (MVP)

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/sensi.git](https://github.com/yourusername/sensi.git)
    cd sensi
    ```
2.  **Upload firmware to microcontroller via Arduino IDE:**
    * Select the correct board & port in Arduino IDE.
    * Flash the `sensi_mvp.ino` file to your microcontroller.
3.  **Pair device with mobile app via Bluetooth** (if applicable): Follow instructions in the companion app.
4.  **Power on and test:**
    * Bring your hand near an obstacle to test proximity feedback.
    * Simulate a loud sound (e.g., clap) to test sound detection feedback.

---

###  Testing & Limitations

* **Obstacle Detection Range:** Current prototype range is approximately 1.5 meters.
* **Sound Classification:** Limited to a small, predefined set of sounds within the MVP scope.
* **Battery Life:** Approximately 6 hours of continuous use (further optimization planned).

---

##  Roadmap

* Expand sound classification capabilities using AI/ML (Edge computing).
* Refine haptic "language" for more nuanced and complex alerts.
* Develop a native Android/iOS companion app with advanced features, including GPS voice-to-vibration translation.
* Improve wearable comfort and implement a waterproof casing.

---

##  Contributing

Contributions, bug reports, and feedback are welcome!
1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature-x`).
3.  Commit your changes (`git commit -am 'Add new feature'`).
4.  Push to the branch (`git push origin feature-x`).
5.  Create a Pull Request.

---

##  License

This project is licensed under the MIT License - see the `LICENSE` file for details.

---

##  Acknowledgements

* Assistive tech pioneers for their inspiring work.
* Open-source communities supporting accessibility innovation.
* Users and testers who provided invaluable feedback during MVP development.

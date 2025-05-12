# 🤖 Mater the Friendly Robot Tow Truck

Welcome to the official code repository for **Mater**, a lovable robotic companion inspired by *Pixar’s Mater* and the expressive *KABANDHA* bot! Mater combines **Bluetooth control**, **servo-powered towing**, and **OLED-based expressions** to create a playful, interactive robot buddy.

This project was built for the [Instructables Robot Friends Contest](https://www.instructables.com/contest/robotfriends/) to demonstrate how personality and functionality can come together in a DIY robot.

---

## 📦 Features

- 🚗 4-Wheel N20 Motor Drive
- 🎮 Bluetooth Control via Android App (HC-05)
- 👁️ Animated OLED Display (robot “eye” expressions)
- 🪝 Servo-Powered Tow Hook
- 🔋 Powered by 7.4V LiPo battery
- 🧠 Dual Arduino Nano architecture for smooth multitasking

---

## 📁 Repository Structure

```

Mater-Robot-TowTruck/
├── Nano1\_MotorControl.ino        # Code for motor + servo control
├── Nano2\_OLED\_Bluetooth.ino     # Code for OLED display + Bluetooth communication
├── wiring\_diagram.jpg            # Optional: Wiring schematic
├── /assets                       # Images or eye animation bitmaps
├── README.md                     # You are here!

````

---

## 🛠️ Hardware Requirements

- 2 × Arduino Nano
- 4 × N20 Motors with Wheels
- 1 × DRV8833 Motor Driver
- 1 × Servo Motor (Tow hook)
- 1 × HC-05 Bluetooth Module
- 1 × OLED Display (128x64, I2C)
- 1 × 7.4V LiPo Battery
- Wires, perfboard, sunboard chassis, and tools (see full Instructable)

---

## 📲 Bluetooth App Setup

Use the **Bluetooth RC Car App** by ANDI.co (available on Android):

1. Pair your HC-05 module (Default PIN: `1234` or `0000`)
2. Use the following commands via the app:

| Command | Action            |
|---------|-------------------|
| F       | Move Forward       |
| B       | Move Backward      |
| L       | Turn Left          |
| R       | Turn Right         |
| S       | Stop               |
| W       | Lift Tow Hook      |
| w       | Lower Tow Hook     |

---

## 💡 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/vanarraj/tom-Mater.git
```
````

2. Open `Nano1_MotorControl.ino` in Arduino IDE → upload to first Nano.

3. Open `Nano2_OLED_Bluetooth.ino` in Arduino IDE → upload to second Nano.

4. Install required libraries:

   * `Servo.h`
   * `Adafruit_GFX.h`
   * `Adafruit_SSD1306.h`

5. Power the system using a 7.4V battery and enjoy Mater's antics!

---

## 🧠 Inspiration & Credits

* Built with inspiration from [Kabandha - The Demon Pet Robot](https://www.instructables.com/member/aphla/)
* Design inspired by Disney Pixar’s *Mater* from *Cars*
* Special thanks to [TheYantracharya](https://www.instructables.com/member/TheYantracharya/) for foundational robotics tutorials

---

## 📸 Showcase

![Mater Demo](assets/mater_demo_.gif)

---

## 📝 License

This project is open-source under the **Attribution Non-commercial (by-nc)**. See [LICENSE](LICENSE) for details.

---

## 🙌 Contributions

Found a bug or want to add features like ultrasonic sensors, sound effects, or obstacle avoidance? PRs and issues are welcome!

---

Happy Hacking! 🚀



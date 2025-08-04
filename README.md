# AUTOMATED CATTLE FEEDER SYSTEM USING IoT

A smart and efficient system designed to automate the feeding of livestock by dispensing food and water at scheduled times using an Arduino-based microcontroller, ensuring timely care, reducing human intervention, and improving farm management, especially in remote or large-scale environments.


# ✅ KEY HIGHLIGHTS

* Real-time scheduling using RTC (DS3231) module
* Servo-controlled food dispensing at pre-set times
* Automated water filling via DC pump
* Relay-controlled power switching for pump
* Arduino microcontroller governs complete operation
* Expandable design for multiple feeding points or animals


# ⚙️ SYSTEM ARCHITECTURE

# Feeding Logic

**Scheduled Operation (e.g., 7:00 AM):**

* RTC module tracks time accurately.
* Arduino checks if the feeding time has been reached.
* Servo motor activates to tilt the feeding cup and release food.
* Relay is triggered to power the water pump and fill the water bowl.
* System uses a flag (`Fed`) to avoid repeated feeding within the same time slot.
* After an hour, the flag is reset for the next scheduled cycle.


#🔩 HARDWARE COMPONENTS

| Component               | Purpose                                      |
| ----------------------- | -------------------------------------------- |
| **Arduino Uno**         | Central controller for the system            |
| **RTC Module (DS3231)** | Keeps track of feeding schedule              |
| **Servo Motor**         | Dispenses food by tilting the feed container |
| **Relay Module**        | Switches the DC pump on/off                  |
| **DC Water Pump**       | Fills the water container                    |
| **Wires, Breadboard**   | Circuit connections                          |


# 💻 SOFTWARE OVERVIEW

# Language

* Arduino C/C++

# Libraries & Modules

* `Wire.h` – I2C communication for RTC
* `RTClib.h` – Interfacing with DS3231 module
* `Servo.h` – Servo motor control
* Custom logic – Feeding schedule and one-time activation flag


# 🔧 FUNCTIONAL FEATURES

* Reads time from RTC module to determine feeding schedule
* Activates servo to dispense food once per cycle
* Powers water pump via relay for a fixed duration
* Prevents repeated feedings using logical flags
* System resets the flag after an hour for continuous daily cycles


# 🛠️ SETUP GUIDE

1. Connect the components as per your hardware schematic.
2. Upload the code to Arduino Uno using the Arduino IDE.
3. Set the RTC time if it has lost power.
4. Power the Arduino via USB or 12V adapter.
5. System will automatically execute the feeding routine at the scheduled time.



# 🚀 FUTURE SCOPE

* Integration with IoT platforms (e.g., Blynk, ThingSpeak) for remote schedule control
* Weight sensor for precise food quantity monitoring
* Mobile notifications and dashboard updates
* Multiple daily feeding routines
* Solar-powered system for off-grid farms


# 📜 LICENSE

This project is open-source and free to use for academic, research, or agricultural innovation purposes.



# 👨‍💻 CONTRIBUTOR

Makeswaran K
Embedded Systems Developer | Smart Agriculture Enthusiast | IoT Innovator

Let me know if you'd like this formatted into a downloadable `.md` file or as a presentation format!

🐄 Automated Cattle Feeder System using IoT
Project By: Makeswaran K, KPR Institute of Engineering and Technology
Guided By: Dr. Jaikumar

🎯 Objective
To build a smart, automated cattle feeding system that delivers food and water at scheduled times using a real-time clock (RTC), reducing manual labor and improving efficiency in livestock management.

🔧 Methodology
🧩 Problem Identification
Recognized the need for automation in livestock feeding, especially in remote or large-scale farming environments where manual effort is impractical.

🔌 System Design
Designed the circuit with the following components:

Arduino Uno – Core microcontroller

RTC Module (DS3231) – Accurate timekeeping

Servo Motor – Controls food dispensing

Relay Module – Controls the water pump

DC Water Pump – Supplies water to livestock

💻 Programming & Logic
Arduino sketch schedules and controls the operation.

RTC ensures feeding occurs precisely at set times.

Servo tilts to release food.

Relay activates the pump to dispense water.

✅ Testing & Validation
Verified scheduled food and water delivery.

Adjusted timing delays for reliable execution.

Ensured system resets daily to prevent repeated feeding within the same hour.

⚙️ Hardware Components
Component	Function
Arduino Uno	Core microcontroller
RTC Module (DS3231)	Maintains accurate feeding time
Servo Motor	Tilts the feeder cup to release food
Relay Module	Switches the DC water pump on/off
DC Water Pump	Fills water bowl for cattle
Wires, Breadboard	Circuit connections and power distribution

🧪 Prototype Functionality
Scheduled Feeding: Servo motor dispenses food at 7:00 AM (configurable).

Timed Watering: Water pump runs for 5 seconds to fill water bowl.

Auto Reset: System resets hourly to prepare for the next feeding cycle.

Scalable: Extendable to feed multiple animals or cover larger farms.

IoT Ready (Future Scope): Supports future integration with cloud platforms for remote control.

💻 Arduino Code Overview
Key Functionalities
Time tracking with RTClib.h

Feed dispensing using Servo.h

Relay-controlled water pumping

Single execution per scheduled time using a flag (Fed)

▶️ How to Run
Assemble the circuit as per the schematic.

Upload the code to the Arduino Uno via the Arduino IDE.

Power the system using USB or an external power supply.

Observe the operation:

At the scheduled time (e.g., 7:00 AM), food is dispensed.

Water pump activates for 5 seconds.

System resets the flag after 1 hour for the next cycle.

🚀 Future Enhancements
Add Wi-Fi/Bluetooth (ESP8266) for IoT-based control.

Integrate load cells to measure food quantity.

Enable multiple feeding schedules throughout the day.

Implement mobile alerts and dashboards using platforms like Blynk or ThingSpeak.

Incorporate solar power for sustainable operation in remote areas.

📜 License
This project is open-source and free to use for academic, research, or agricultural automation purposes.

👨‍💻 Contributor
Makeswaran K
IoT Developer | Embedded Systems Enthusiast | Agriculture Innovator


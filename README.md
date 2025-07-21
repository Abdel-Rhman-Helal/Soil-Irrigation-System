# Soil Irrigation System using ATmega32 Microcontroller

## Project Summary

The **Soil Irrigation System** is a smart embedded solution designed to improve agricultural efficiency by automating water delivery based on soil moisture levels. Powered by an ATmega32 microcontroller, this system makes real-time decisions to maintain optimal moisture conditions for plant growth. It supports both automatic operation and user-configurable scheduling through a keypad interface, while also providing data logging through UART communication to a connected computer.

---

## Key Functionalities

- **Automatic Irrigation Mode**  
  Continuously monitors soil moisture levels and turns on the water pump when the moisture drops below a set threshold—no manual input required.

- **Custom Interval Scheduling**  
  Users can configure watering intervals using a 4x4 keypad. The system irrigates based on the specified schedule and real-time moisture readings.

- **Serial Data Reporting**  
  Sends live soil moisture readings via UART to a computer for visualization and logging. A Python script processes the incoming data for monitoring and analysis.

---

## Required Hardware

- ATmega32 Microcontroller  
- Soil Moisture Sensor(s)  
- 16x2 LCD Display  
- 4x4 Keypad  
- Relay Module  
- DC Water Pump  
- External Power Supply  
- Serial Communication Cable (for UART)

---

## Microcontroller Features Utilized

- **ADC (Analog-to-Digital Converter)**  
  Converts analog signals from the moisture sensors into digital values the microcontroller can process.

- **Timers**  
  Enables timed irrigation intervals in the user-defined mode.

- **UART**  
  Facilitates communication between the ATmega32 and an external PC for live data transfer.

---

## Software Overview

- **Firmware (C Language)**  
  The microcontroller code manages sensor inputs, relay control, LCD output, keypad handling, and UART communication.

- **Python Script (PC Side)**  
  A simple Python script reads serial data from the microcontroller and displays or stores moisture readings for analysis.

---

## How to Set Up

### Required Materials

Before starting, make sure you have the following:

- ATmega32 development board or circuit
- USBasp or other AVR programmer
- Moisture sensors and compatible relay module
- 16x2 LCD and 4x4 matrix keypad
- External power supply (suitable for pump and controller)
- Python installed on your computer (along with `pyserial`)

### Operating Instructions

#### ➤ Automatic Mode
- Power up the system.
- The pump will activate only when the soil becomes too dry.

#### ➤ Manual Scheduling Mode
- Use the keypad to enter the desired irrigation interval.
- The system will check moisture and irrigate periodically based on the set duration.

---

## Wiring Diagram

<img width="807" height="631" alt="image" src="https://github.com/user-attachments/assets/b7a78e83-0e99-49b1-9e4b-2d3dc31fba8f" />


The above diagram represents the full circuit used in the system, including the sensor, relay, LCD, and keypad interfaces with the ATmega32.

---

## Project Highlights

- **Fully Automated Control**  
  Requires no user intervention in default mode.

- **Custom Scheduling**  
  Flexibility for timed irrigation based on user preference.

- **Real-Time Monitoring**  
  Moisture data can be recorded and visualized externally using Python tools.

---

This project blends embedded control and basic data visualization to solve a real-world agricultural problem. Ideal for students, hobbyists, or engineers exploring microcontroller-based automation systems.

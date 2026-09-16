# Energy Consumption Monitoring System

An Arduino-based embedded system designed to monitor **voltage, current, power, and energy consumption in real time**.

This project was developed as a **Public Interest Design (PID)** project, focusing on making energy information more accessible and understandable while encouraging more responsible electricity consumption.

---

## Project Overview

The Energy Consumption Monitoring System uses an Arduino Uno, voltage and current sensors, and an LCD display to measure and analyse electricity usage.

The system continuously collects electrical measurements and calculates:

- Voltage (V)
- Current (A)
- Power (W)
- Energy consumption (kWh)
- Energy usage percentage
- Energy efficiency status

The measurements are displayed locally on an LCD screen, allowing users to see their energy usage in real time.

---

## Project Objective

The main objective is to develop a simple, affordable, and easy-to-understand energy monitoring system that can help users become more aware of their electricity consumption.

The system demonstrates how embedded systems can be applied to everyday energy-management problems.

---

## Components

| Component | Purpose |
|---|---|
| Arduino Uno | Microcontroller |
| Voltage Sensor | Measures voltage |
| Current Sensor | Measures current drawn by the load |
| LCD Display | Displays energy measurements |
| LED | Visual indicator |
| Resistor | Used with the LED |
| Breadboard | Prototyping |
| Jumper Wires | Electrical connections |

The prototype uses a simple circuit consisting of an LED and resistor as the load to be monitored.

---

## How It Works

### 1. Input

The voltage and current sensors continuously monitor the electrical characteristics of the load.

### 2. Processing

The Arduino Uno samples the sensor signals and calculates electrical parameters.

Power is calculated using:

**P = V × I**

The system also calculates cumulative energy consumption in kWh.

### 3. Output

The calculated values are displayed on the LCD screen.

The system compares energy usage against a programmed benchmark and displays an efficiency status.

```text
Voltage Sensor ──┐
                 │
Current Sensor ──┼──> Arduino Uno ──> LCD Display
                 │
      Load ──────┘

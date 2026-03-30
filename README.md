# Digital Thermometer with I2C LCD Display

## 📌 Project Overview
This project is an embedded system designed to monitor real-time ambient temperature using an **Arduino Uno** and a **TMP36 sensor**. The data is processed and displayed on a **16x2 LCD screen** using the **I2C communication protocol** to minimize wiring complexity.

## 🎯 Objectives
* Interface a TMP36 temperature sensor with an Arduino using analog input.
* Implement I2C communication to control a 16x2 Liquid Crystal Display.
* Convert raw analog voltage data into human-readable Celsius values.
* Provide real-time status updates via the serial monitor and LCD.

## 🛠️ Components & Tools
* **Microcontroller:** Arduino Uno R3
* **Sensor:** TMP36 Analog Temperature Sensor
* **Display:** 16x2 LCD with I2C Backpack (PCF8574)
* **Simulation Platform:** Tinkercad
* **Language:** C++ (Arduino Sketch)

## 🔌 Circuit Connections
| Component Pin | Arduino Pin | Description |
| :--- | :--- | :--- |
| **TMP36 Vout** | **A0** | Analog Temperature Signal |
| **I2C LCD SDA** | **A4** | Serial Data Line |
| **I2C LCD SCL** | **A5** | Serial Clock Line |
| **VCC / 5V** | **5V Rail** | Positive Power Supply |
| **GND** | **GND Rail** | Ground |

## 🚀 How to Run
1. **Clone this repository** to your local machine.
2. **Open the `.ino` file** in the Arduino IDE.
3. **Install the Adafruit LiquidCrystal library** via the Library Manager.
4. **Upload the code** to your Arduino Uno.
5. **(Optional)** Import the circuit design into **Tinkercad** to run the simulation virtually.

## 📝 Code Logic
The system reads the analog value from the TMP36, which provides a voltage proportional to the temperature. The software applies the following formula to calculate degrees Celsius:

$$(Voltage - 0.5) \times 100 = Temperature (°C)$$

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.

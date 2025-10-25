# ⚡ ESP32-Controlled Lab Power Supply

A smart, programmable **lab power supply** controlled by an **ESP32 microcontroller**.  
This project combines hardware design and firmware development to provide precise, remote control over voltage and current using a **custom-designed PCB**.

---

## 🧠 Project Overview

This project was created to make a standard lab power supply smarter and easier to use.  
By adding an ESP32 and a custom interface board, I was able to control voltage, current, and safety features remotely — either through a web dashboard, serial commands, or a mobile app.

The repository includes both the **ESP32 firmware** and **PCB schematics** for full reproducibility.

---

## ⚙️ Features

- **Precise Voltage and Current Control**  
  Adjust and monitor power output in real time with fine-grained accuracy.

- **Multiple Control Interfaces**  
  Control the supply through a web interface, serial monitor, or a custom mobile app.

- **Programmable Output Profiles**  
  Automate experiments by predefining voltage/current sequences.

- **Built-in Safety Protections**  
  Includes software-based overvoltage and overcurrent protection to safeguard connected devices.

- **Custom PCB Design**  
  Handles signal conditioning and power control between the ESP32 and the lab power supply.

---

## 🧩 Components Used

| Component | Description |
|------------|-------------|
| **ESP32 DevKit** | Main controller, handles communication and web interface |
| **Custom PCB** | Connects ESP32 to lab supply, includes signal conditioning and protection |
| **Lab Power Supply** | Provides adjustable voltage and current output |
| **MOSFETs, Diodes, Resistors, Capacitors** | Used for power regulation and switching |
| **Connectors & Headers** | For input/output and debugging connections |

---

## 🔌 Schematics

The schematic below shows how the ESP32 interfaces with the lab power supply via the custom PCB.

![image](https://github.com/user-attachments/assets/3d6ff594-d53d-4782-9ef0-390cf0411aab)

---

## 💻 Firmware

The ESP32 firmware handles communication, user commands, and power control logic.

- Written in **C++** using the **Arduino framework**
- Communicates with the lab supply over digital I/O and serial protocols
- Supports **web-based control** via Wi-Fi and **serial communication**
- Implements **PID-style regulation** for smooth voltage and current control

### 🔧 Installation

1. Install the **Arduino IDE** or **PlatformIO** with ESP32 board support.  
2. Clone this repository.  
3. Open the firmware folder in your IDE.  
4. Compile and upload the code to the ESP32 board.  
5. Connect the ESP32 to the custom PCB and power supply.  

---

## 🧱 PCB Design

### 🧾 Production

Gerber files for PCB manufacturing are included in this repository.  
You can upload them directly to any PCB fabrication service (e.g., JLCPCB, PCBWay).

### 🔩 Assembly

Solder the through-hole and SMD components as labeled on the silkscreen.  
Pay attention to MOSFET orientation and connector alignment.

![image](https://github.com/user-attachments/assets/2623b5b7-6240-4525-8b95-48c2bddd8577)



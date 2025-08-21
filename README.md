# 🏠 Home Automation System with ESP32

## 📘 Project Overview

This project presents a smart home automation system developed for the **Electronics and Communication Engineering (ECE) Department Project Lab**. The system enables users to control electrical appliances in real-time using a **web dashboard**, while also offering manual control through physical switches. It is based on the **ESP32 microcontroller**, with full integration to **Google Cloud** and **Arduino IoT Cloud**, ensuring secure, scalable, and dynamic operation.

### 🔑 Key Highlights

- ✅ ESP32-based home automation with web-based control  
- 🔐 Google Cloud Smart Variables used for secure cloud communication  
- 🔀 Two-way switch system: control via both physical switches and web dashboard (only when online)  
- 🌐 Dynamic Wi-Fi credential management through onboard web portal using WiFiManager  
- 📡 Real-time monitoring and synchronization of switch states

---

![Home Automation System](https://github.com/ArijitDutta96395/Home_Automation/blob/main/home_automation.png)  
*Home Automation Setup*


---
## 🧰 Hardware Components

| 🔩 Component       | 📝 Description                                                            |
| ----------------- | ------------------------------------------------------------------------ |
| 🧠 ESP32           | The main controller that connects to the cloud and controls the relays   |
| ⚡ Relay Modules   | Used to control AC appliances like lights and fans                       |
| 🖲️ Manual Switches | Allows manual toggle of appliances (requires internet connection)        |
| 🔌 Power Supply    | A regulated power adapter to power the ESP32 and relays                  |

---

## 🛠️ Software and Cloud Services

| 💻 Tool/Service                   | 📈 Role in the System                                  |
| ------------------------------- | ------------------------------------------------------ |
| 🧑‍💻 Arduino IDE                  | Firmware development and uploading to ESP32            |
| ☁️ Arduino IoT Cloud              | Real-time monitoring and control interface             |
| 🛡️ Google Cloud (Smart Variables) | Secure cloud communication and device state storage    |
| 📶 WiFiManager Library            | Web portal for dynamic Wi-Fi configuration             |
| 🗣️ Google Home (optional)         | Planned integration for voice control                  |

---

## ⚙️ Features and Working

### 🔌 Appliance Control

The ESP32 controls electrical appliances through relay modules. Users can control these relays using the **Arduino IoT Cloud Web Dashboard**. The status of each appliance is updated in real-time.

### 🔁 Two-Way Switch System (Online Mode Only)

When connected to the internet, appliances can be controlled using either:

- 🖥️ **Web Dashboard** (primary control)  
- 🧲 **Manual Switches** (secondary control)

If a user toggles an appliance manually, the web dashboard reflects the updated state instantly.

### 📲 Dynamic Wi-Fi Configuration

Using **WiFiManager**, users can update Wi-Fi credentials without reprogramming the ESP32. On first-time setup or Wi-Fi failure, the ESP32 launches a **web portal** where users can input new credentials through a browser.

---

## 🔄 How the System Works

1. 🔍 On boot, the ESP32 checks for stored Wi-Fi credentials. If missing or invalid, it hosts a captive web portal using WiFiManager.  
2. 🌐 Once connected to Wi-Fi, the ESP32 connects to the Arduino IoT Cloud and syncs with Smart Variables.  
3. 🔗 Appliance control is handled through relay modules, which respond to commands from:  
   - 🖥️ Arduino Web Dashboard  
   - 🧲 Physical switches (only when internet is available)  
4. 🔄 Switch state is reflected in real-time on the dashboard, keeping both manual and web control in sync.

---

## 🖼️ Screenshots

> ![ESP32 + Relay Hardware Setup](https://github.com/user-attachments/assets/f7d27083-8020-4ac8-b361-828aa47420b5)  
> ![Arduino IoT Cloud Web Dashboard Interface](https://github.com/user-attachments/assets/0d858bc9-0629-4242-a177-d6caa0bfc27d)

📷 **Images:**
- ESP32 + Relay Hardware Setup  
- Arduino IoT Cloud Web Dashboard  
- WiFiManager Captive Portal

---

## 🚀 Getting Started

### ✅ Prerequisites

- 🖥️ Arduino IDE installed on your system  
- 🧠 ESP32 board package added to Arduino IDE  
- ☁️ Arduino IoT Cloud account and credentials  
- 📦 Required libraries:  
  - `WiFiManager`  
  - `ArduinoIoTCloud`  
  - `Arduino_ConnectionHandler`

### 🔧 Installation

### Installation

1. Clone the repository:

   ```
   git clone https://github.com/Avijit89n/Home-Automation-ESP32.git
   ```

2. Open the `.ino` file in Arduino IDE.

3. Replace placeholders with your **Device ID**, **Secret Key**, and **Cloud Variables** from Arduino IoT Cloud.

4. Upload the code to the ESP32 using a USB connection.

5. On first boot, the ESP32 will open a WiFiManager portal. Connect to it using a smartphone or PC and enter the desired Wi-Fi credentials.

6. Once connected, visit the Arduino IoT Cloud dashboard to control appliances remotely.

---

## Future Enhancements

* Enable offline switch synchronization using local memory
* Add voice command integration with Google Home or Alexa
* Create a dedicated mobile app for enhanced user experience
* Integrate power usage tracking and analytics

---

## License

This project is licensed under the **MIT License**.
Refer to the [LICENSE](./LICENSE) file for full terms and conditions.

---

## Author

**Arijit Dutta**
Electronics and Communication Engineer
Specializing in Embedded Systems and IoT Applications
Email: \[[optional@example.com](mailto:optional@example.com)]
GitHub: [github.com/ArijitDutta96395](https://github.com/ArijitDutta96395)


   ```bash
   git clone https://github.com/ArijitDutta96395/Home_Automation.git

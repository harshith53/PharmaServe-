# 🚀 PHARMA SERVE: IoT-Based Medicine Pill Drop System  

## 🏥 Overview  
PHARMA SERVE is an **IoT-based automated pill dispensing system** designed using the **ESP8266 (NodeMCU)**. It detects motion using a **PIR sensor**, controls a **servo motor** for pill dispensing, and triggers a **buzzer** for alerts. The system displays the **time and date on an LCD screen**, synchronized via an **NTP server** for accuracy. It also supports **remote monitoring and control via the Blynk app**, making it a **smart and user-friendly healthcare solution**.  

---

## 🛠️ Components Used  
- **ESP8266 Wi-Fi Module** – (NodeMCU) for connectivity  
- **PIR Motion Sensor** – Detects motion  
- **Servo Motor** – Dispenses pills  
- **Buzzer** – Alerts on motion detection  
- **LCD (16x2) with I2C** – Displays real-time date & time  
- **Blynk App** – Remote monitoring & control  
- **NTP Server** – Ensures accurate time synchronization  

---

## ✨ Features  
✅ **Motion Detection** – Detects movement via PIR sensor  
✅ **Automated Pill Dispensing** – Servo motor dispenses medicine  
✅ **Alert System** – Buzzer sounds upon detection  
✅ **Remote Monitoring & Control** – Via Blynk app  
✅ **Real-Time Time Display** – Synced with an NTP server  
✅ **User-Friendly Interface** – Easily view and control through the LCD & app  

---

## 📌 Pin Connections  

| Component        | GPIO Pin |  
|-----------------|----------|  
| PIR Sensor      | GPIO 12  |  
| Servo Motor     | GPIO 13  |  
| Buzzer         | GPIO 14  |  
| LCD Display (I2C) | Address `0x27` (16x2) |  

---

## 📚 Libraries Used  
Make sure you have these **Arduino libraries** installed:  
- `ESP8266WiFi.h` – Connects ESP8266 to Wi-Fi  
- `BlynkSimpleEsp8266.h` – Blynk integration  
- `LiquidCrystal_I2C.h` – LCD control  
- `Servo.h` – Controls the servo motor  
- `NTPClient.h` – Fetches real-time from an NTP server  
- `WiFiUdp.h` – Handles UDP communication for NTP  

---

## 📲 Blynk App Setup  
1. **Create a new project** in the **Blynk app**  
2. **Get the Auth Token** from Blynk & replace it in the code (`#define BLYNK_AUTH_TOKEN`)  
3. **Add the following widgets**:  
   - **V2** – Controls Buzzer  
   - **V3** – Controls Servo Position  
   - **V4** – Additional Buzzer Control  
   - **V5** – Displays motion detection status  

---

## 🚀 Steps to Run  
1. **Hardware Setup** – Wire all components as per the pin connections  
2. **Install Required Libraries** – Ensure all the mentioned libraries are installed  
3. **Upload the Code** – Flash the code onto the **ESP8266** using the **Arduino IDE**  
4. **Connect to Wi-Fi** – Ensure the ESP8266 is connected  
5. **Start Blynk App** – Open the Blynk app & control the system remotely  

---

## 🛠️ Code Functionality  
- **Wi-Fi & Time Sync:** ESP8266 connects to Wi-Fi and fetches time via an **NTP server**  
- **Pill Dispensing:** PIR sensor detects motion → Activates servo → Dispenses medicine  
- **Alert System:** Buzzer alerts when motion is detected  
- **Display Updates:** LCD shows real-time **time & motion status**  
- **Blynk Control:** The app allows remote **monitoring & control** of servo and buzzer  

---

## ❗ Troubleshooting  
- **Wi-Fi Issues?** – Double-check your **Wi-Fi credentials** in the code  
- **Servo Not Moving?** – Ensure it’s connected to the **correct GPIO pin**  
- **LCD Not Displaying?** – Check **I2C wiring & address** (`0x27`)  
- **Blynk Not Responding?** – Verify your **Auth Token is correctly set**  

---

## 📜 License  
This project is **open-source** and can be modified for **personal and educational** use.  

💡 *Feel free to contribute and improve PHARMA SERVE!* 🚀

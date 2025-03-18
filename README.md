# 🌱 Automatic Soil Irrigation System using IoT  

## 📌 Project Description  
This project is an **IoT-based smart irrigation system** that monitors soil moisture levels and automatically controls a **water pump** based on real-time sensor readings. It also measures **temperature and humidity** using a **DHT11 sensor** and sends alerts via **Blynk notifications**.  

---

## 🔧 Technologies & Components Used  
- **Microcontroller:** ESP8266  
- **Sensors:**  
  - **DHT11** (Temperature & Humidity Sensor)  
  - **Soil Moisture Sensor**  
- **Actuator:** Water Pump & Relay Module  
- **Communication:** Wi-Fi (ESP8266)  
- **Cloud Platform:** Blynk App for remote monitoring  
- **Software Tools:** Arduino IDE  

---

## 🚀 Features  
✅ **Monitors soil moisture, temperature, and humidity in real-time**  
✅ **Automatically turns ON/OFF the water pump based on moisture level**  
✅ **Remote monitoring & alerts via Blynk notifications**  
✅ **Wi-Fi-based smart agriculture solution**  

---

## 🛠️ How It Works  
1️⃣ The ESP8266 reads **soil moisture data** from the **moisture sensor**.  
2️⃣ It also records **temperature & humidity** from the **DHT11 sensor**.  
3️⃣ If the **moisture level is low (<50%)**, the **water pump is activated**.  
4️⃣ If the moisture level is **>56%**, the **pump is turned OFF**.  
5️⃣ All data is sent to the **Blynk cloud**, and a notification is triggered.  

---

## 📜 Code Explanation  
- **`dht.readTemperature()` & `dht.readHumidity()`** → Reads temperature & humidity data.  
- **`analogRead(moisturePin)`** → Measures soil moisture level.  
- **Motor Control Logic:**  
  - If **moisture < 50%**, the motor **turns ON**.  
  - If **moisture > 56%**, the motor **turns OFF**.  
- **Blynk Integration:**  
  - Sends real-time notifications:  
    `"Moisture: XX%, Temp: XX°C, Humidity: XX%"`  

---

## 📷 Circuit Diagram  
![circuit](https://github.com/user-attachments/assets/2cbd5de0-ab29-4bf6-9e1a-b3e2a383dd1a)
 

---

## 🚀 How to Run the Project  
1️⃣ **Upload the code to ESP8266** using **Arduino IDE**.  
2️⃣ **Connect the hardware components** as per the circuit diagram.  
3️⃣ **Update the Wi-Fi credentials & Blynk auth token** in the code.  
4️⃣ **Monitor sensor values & control the system** via **Blynk App**.  

---



---


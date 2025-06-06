# 🌫️ Standalone Air Pollution Monitoring for Stone Crushing Operation Plant using STM32

This project is a standalone embedded system designed to **monitor air quality** in hazardous industrial environments—particularly stone crushing operation plants—where dust and gas pollutants are commonly present. Built using the **STM32F401RE Nucleo board**, the system detects harmful gases and alerts nearby workers in real-time.

## 📌 Key Features

- 🔬 **Gas Detection:** MQ-135 sensor detects pollutants like CO₂, NH₃, benzene, and more.
- 🧠 **Microcontroller:** STM32F401RE handles all processing and interfacing.
- 🌡️ **Temperature Monitoring:** LM35 sensor for ambient temperature.
- 👁️ **Human Presence Detection:** LDR-based detection to identify nearby workers.
- 🔔 **Alert System:** Buzzer/LED alert when unsafe conditions are detected.
- 💬 **Serial Output:** USART communication sends real-time messages to a PC or terminal.
- ⚡ **Standalone System:** No need for internet/cloud services — perfect for remote environments.

## 🛠️ Hardware Used

- STM32F401RE Nucleo Board  
- MQ-135 Gas Sensor  
- LM35 Temperature Sensor  
- LDR (Light Dependent Resistor)  
- Buzzer / LED  
- Custom PCB  
- USB Power Supply

## 💡 Working Principle

- MQ-135 continuously monitors air pollutants.
- LDR detects human presence near the device.
- STM32 reads analog values, checks thresholds, and triggers alerts if pollution + presence conditions are met.
- Message is transmitted via USART and LED/Buzzer is activated.
- The system loops continuously for real-time protection.

## 🧪 Output Example

```text
Fresh AIR
Unhealthy AIR - Move To Safe Zone

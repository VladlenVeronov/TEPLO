# TEPLO
TEPLO: Smart Heating System Control**   TEPLO is a Flutter-based app for managing heating systems via an ESP32-powered device. Control and monitor temperature remotely over Wi-Fi or IP, adjust settings, and view operational data. Built for efficiency and remote access, TEPLO brings smart, decentralized climate control to your fingertips.

**TEPLO: Smart Heating System Control App**

TEPLO is a Flutter-based mobile application designed to manage heating systems, giving users complete control over their indoor climate via Wi-Fi or remote IP access. Built around a custom device architecture powered by the ESP32 module, TEPLO enables users to monitor and adjust temperature settings, check device status, and view operational data, all from their smartphone.

### About the Device

The TEPLO device is engineered to manage heating systems effectively and efficiently. Using an ESP32 microcontroller as its core, it integrates multiple components to enable precise temperature control and real-time monitoring. The device connects seamlessly with Wi-Fi, allowing users to control heating settings locally and, with additional IP configuration, from anywhere in the world. Users can view system status, adjust operational settings, and customize preferences directly from the TEPLO app.

### Key Components

1. **ESP32 Microcontroller (ESP32-WROOM-32U)**  
   Manages data collection, relay operation, Wi-Fi connection, and request processing.

2. **5V 30A Relay**  
   Controls the heating system's power based on temperature thresholds.

3. **NTC Thermistor (10kΩ)**  
   Measures temperature; connected to ESP32’s analog input to read temperature-dependent resistance.

4. **10kΩ Resistor**  
   Works with the thermistor in a voltage divider to measure temperature-related voltage changes.

5. **LCD 1602 Display with I2C Interface**  
   Shows current and target temperatures and time information for quick reference.

6. **Power Supply (5V or 9.6V, minimum 4.8W)**  
   Supplies stable power to the ESP32 and relay modules.

7. **AMS1117 Voltage Converter**  
   Steps down voltage from 9.6V to 5V for stable ESP32 and relay operation.

8. **Diode (e.g., 1N4007)**  
   Protects against reverse inductive surges during relay switching.

9. **MOSFET Transistor (IRFZ44N or similar)**  
   Regulates relay power supply; handles power that ESP32 alone cannot supply.

10. **Pull-up Resistor for BOOT Button**  
    BOOT button serves as a manual control for the LCD display.

11. **Ceramic Capacitors (100nF, 1nF)**  
    Filters input power for ESP32 and relay stability.

12. **Software**  
    - **Arduino IDE** for programming the ESP32 microcontroller.
    - **Flutter** or **FlutterFlow** for the mobile application, which communicates with the device and displays data to users.

13. **Database Integration**  
    Tracks device status and sends updated settings remotely without direct IP connection.

### Application Features

- **Real-time Temperature Monitoring**: View current and target temperature data directly from the device.
- **Remote Control**: Manage heating settings locally over Wi-Fi or globally via IP.
- **Operational Status**: Check device activity, runtime, and diagnostic data.
- **Custom Settings**: Modify temperature preferences, operation schedules, and other settings according to user needs.

### How TEPLO Works

The app communicates with the ESP32-based device, allowing users to monitor and control their heating systems remotely. It uses the NTC thermistor to capture real-time temperature data, the relay to control the heating system, and an LCD screen for instant data display. With a stable power supply and an efficient relay system, TEPLO operates reliably to deliver responsive heating control from anywhere.

### Future Development

This repository serves as a foundation for building and expanding upon TEPLO. Additional functionality and enhancements can be implemented to improve device features, refine user experience, and support further integration.

### Technologies Used

- **Microcontroller**: ESP32 (ESP32-WROOM-32U)
- **Mobile App**: Flutter (Dart language)
- **Programming**: Arduino IDE for ESP32
- **Database**: For remote state tracking and settings updates

TEPLO redefines home heating control, making it smarter, more efficient, and accessible from any location.

---
### English Version
All rights to the code are owned by VR-GROUP DEVELOPERS LLC.

The code is permitted for personal, non-commercial use only. Commercial use, distribution, modification, or integration of this code into commercial products or services is strictly prohibited without prior permission from VR-GROUP DEVELOPERS LLC.

VR-GROUP DEVELOPERS LLC reserves the right to modify the code and licensing terms with each new version of the website.

If you intend to use this code for commercial purposes, please contact VR-GROUP DEVELOPERS LLC to obtain permission. To do so, submit a request through the provided contact information. All usage terms will be agreed upon by mutual consent.

Contact Information:
- Company Director: Vladyslav Novytskyi, Ukraine.
- Website: [vr-group.io](https://vr-group.io)
- Inquiries and feedback: [service@vr-group.io](mailto:service@vr-group.io)

This license is effective from the moment this code is used and may be modified by VR-GROUP DEVELOPERS LLC at any time without prior notice.

###License Version
This is the first version of the license, issued on November 14, 2024.


---

## Ліцензія (Версія 1.0 від 14.11.2024)

### Українська версія
Всі права на код належать товариству з обмеженою відповідальністю VR-GROUP DEVELOPERS LLC.

Дозволяється використовувати цей код тільки для особистого, аматорського використання. Комерційне використання, розповсюдження, модифікація або інтеграція коду в комерційні продукти або сервіси суворо заборонено без попереднього дозволу від VR-GROUP DEVELOPERS LLC.

ТОВ ВР-ГРОУП ДЕВЕЛОПЕРС залишає за собою право змінювати код та ліцензійні умови з кожною новою версією сайту.

Якщо ви маєте намір використовувати цей код у комерційних цілях, зверніться до ТОВ ВР-ГРОУП ДЕВЕЛОПЕРС для отримання відповідного дозволу. Для цього надішліть заяву за вказаними контактами. Усі умови використання будуть узгоджені за домовленостями.

Контактна інформація:
- Керівник компанії: Владислав Новицький, Україна.
- Вебсайт: [vr-group.io](https://vr-group.io)
- Питання та побажання: [service@vr-group.io](mailto:service@vr-group.io)

Ця ліцензія набуває чинності з моменту використання цього коду та може бути змінена ТОВ ВР-ГРОУП ДЕВЕЛОПЕРС у будь-який час без попереднього повідомлення.

### Версія ліцензії
Це перша версія ліцензії, випущена 14 листопада 2024 року.


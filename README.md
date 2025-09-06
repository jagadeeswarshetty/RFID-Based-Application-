RFID-Based Smart Access and Inventory System
📝 About the Project

The RFID-Based Smart Access and Inventory System is a microcontroller-based prototype that combines authentication and inventory management into a single solution. Using an Arduino Uno and an RFID reader (RC522), the system reads RFID tags/cards and makes decisions based on predefined access rights or inventory status.

This project was developed to demonstrate how IoT and embedded systems can improve security, automation, and data accuracy in real-life applications. It is an entry-level project but can be scaled into industrial or IoT-based solutions.

📖 Project Information
🔹 Objectives

To implement RFID-based authentication for secure access control.

To automate inventory logging and tracking of items.

To reduce manual intervention and human error.

To create a low-cost and scalable system that can integrate with IoT platforms in the future.

🔹 System Workflow

Initialization – The Arduino boots up and initializes the RFID reader, LCD, buzzer, and LEDs.

Card Scan – A user scans an RFID card or an item with an RFID tag.

Verification – The system reads the UID (Unique ID) of the tag and compares it with stored authorized IDs.

Decision –

✅ If the UID matches → Access Granted / Item Logged IN or OUT.

❌ If the UID doesn’t match → Access Denied.

Logging – All attempts are recorded on the Serial Monitor (can be extended to a database).

🔹 Features

Real-time authentication with RFID cards/tags.

User feedback using buzzer, LED, and LCD display.

Logging capability for access and inventory events.

Modular design – can be integrated with database, IoT dashboards, or relays for controlling doors/locks.

🔹 Applications

Smart Door Lock Systems (offices, hostels, labs).

Library Management (issue/return books using RFID).

Warehouse Inventory Tracking (logging stock IN/OUT).

Attendance System (student or employee tracking).

🔹 Advantages

🔒 Enhanced security using RFID authentication.

⏱️ Time-saving compared to manual systems.

📉 Error reduction in record-keeping.

💡 Scalable – can integrate with IoT/cloud solutions.

💰 Low-cost hardware implementation.

🛠️ Components Used

Arduino Uno / Nano

MFRC522 RFID Reader

RFID Tags / Cards

16x2 LCD Display (I2C interface)

Buzzer

Red & Green LEDs

Breadboard + Jumper wires

🔧 Circuit Connections
Component	Arduino Pin
RC522 SDA (SS)	D10
RC522 RST	D9
RC522 MOSI	D11
RC522 MISO	D12
RC522 SCK	D13
Buzzer	D3
Green LED	D4
Red LED	D5
LCD (I2C) SDA	A4
LCD (I2C) SCL	A5
📂 Project Structure
RFID-Access-Inventory/
│── code/
│   └── rfid_access_inventory.ino     # Arduino source code
│── docs/
│   └── circuit_diagram.png           # Circuit diagram image
│── README.md                         # Project documentation

🔮 Future Improvements

🔗 Database Integration – Store logs in MySQL, Firebase, or cloud.

📶 IoT Dashboard – Monitor access/inventory via web or mobile app.

🔐 Relay & Electronic Lock – Control physical doors.

💾 SD Card Module – Store logs offline.




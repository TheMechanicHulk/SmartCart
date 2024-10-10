# SmartCart: Seamless Shopping Experience Integration with RFID and Mobile App

## Overview
The SmartCart project aims to enhance the shopping experience by integrating a smart shopping cart with RFID technology and a mobile application. Developed as part of my Bachelor Thesis, this system allows customers to easily scan items, view product details, and manage their shopping list seamlessly. The integration of Arduino and Raspberry Pi ensures real-time updates and efficient inventory management.

## Features
- **RFID Integration**: Automatically detects items placed in the cart using RFID tags, reducing manual scanning effort.
- **Mobile Application**: A user-friendly mobile app that allows customers to scan items and view detailed product information.
- **Real-Time Updates**: The system dynamically updates the total amount and item count on both the mobile app and LCD screen.
- **Inventory Management**: Reflects changes in the inventory database in real-time, ensuring accurate stock levels.

## Workflow
1. **Item Scanning**: Customers can scan items using the mobile app, which communicates with the shopping cart.
2. **RFID Detection**: RFID technology automatically adds items to the shopping list if not manually scanned.
3. **Dynamic Updates**: The mobile app and LCD screens display the updated total amount and item count.
4. **Database Synchronization**: Changes in inventory are reflected in real-time in the backend database.

## Implementation Details
- **Technologies Used**:
    - **Arduino**: For interfacing with RFID readers and managing cart functionalities.
    - **Raspberry Pi**: To host the backend services and database for inventory management.
    - **Mobile App**: Developed using [specific mobile app framework, e.g., Flutter, React Native].

- **Components**:
    - `arduino_code.ino`: Arduino code for RFID scanning and cart management.
    - `raspberry_pi_server.py`: Backend server code running on Raspberry Pi for handling requests and database updates.
    - `mobile_app/`: Source code for the mobile application.

## Installation and Setup
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/TheMechanicHulk/SmartCart.git
    cd SmartCart
    ```

2. **Arduino Setup**:
    - Connect the RFID reader and other necessary components to the Arduino.
    - Upload the `arduino_code.ino` sketch to the Arduino board.

3. **Raspberry Pi Setup**:
    - Ensure you have Python installed on your Raspberry Pi.
    - Run the backend server:
    ```bash
    python raspberry_pi_server.py
    ```

4. **Mobile App Setup**:
    - Open the mobile app project in your preferred development environment.
    - Follow the instructions in the mobile app documentation to build and run the application.

## Project Structure
```bash
├── arduino_code.ino     # Arduino code for RFID scanning and cart management
├── raspberry_pi_server.py # Backend server code for inventory management
└── mobile_app/          # Source code for the mobile application

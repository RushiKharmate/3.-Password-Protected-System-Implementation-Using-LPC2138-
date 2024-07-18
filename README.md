# Password Protected System Using LPC2138 with UART Communication

## Project Overview

This project demonstrates a password-protected system using two LPC2138 microcontrollers with UART communication. The system features a keypad for password entry, an LCD display for user feedback, and a motor that operates based on the password verification.

## Components

- 2x LPC2138 microcontrollers
- 2x LM016L LCD displays
- Keypad
- DC motor
- Push buttons
- HC-05 Bluetooth module for UART communication

## Functionality

1. **Password Entry**: The master microcontroller reads a password entered via the keypad.
2. **UART Communication**: The master microcontroller sends the entered password to the slave microcontroller using UART.
3. **Password Verification**: The slave microcontroller compares the received password with a pre-defined password.
4. **Feedback and Motor Control**: The slave microcontroller sends a success or failure response back to the master. Based on the response, the master microcontroller displays appropriate messages on the LCD and controls the motor.

## How to Use

1. **Setup**:
    - Connect the components as per the circuit diagram.
    - Ensure the UART communication lines (TX and RX) are properly connected between the two LPC2138 microcontrollers.

2. **Programming**:
    - Load the master code (`master_code.c`) onto the master LPC2138 microcontroller.
    - Load the slave code (`slave_code.c`) onto the slave LPC2138 microcontroller.

3. **Operation**:
    - Power on the system.
    - Enter the password using the keypad on the master device.
    - The master device will send the password to the slave device via UART.
    - The slave device will verify the password and send back a success or failure response.
    - The master device will display the result on the LCD and operate the motor accordingly.
      
## Contact

   - Author: [Rushi Kharmate]
   - Email: [rushirajekharmate@gmail.com]


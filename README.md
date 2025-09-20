# 🔐 STM32 Custom Bootloader

A **custom bootloader for STM32 microcontrollers**, featuring support for UART communication, flash memory operations, and secure transitions to user applications. The implementation was carried out on the STM32L496ZG-P Nucleo development board and HAL.

---

## 🚀 Features
- Bootloader / User App mode selection (via button press)  
- UART command interface with ACK/NACK protocol  
- CRC32 check for packet integrity  
- Flash erase & memory write support  
- Jump to user application with MSP + VTOR remap  
- Debug logging on secondary UART  

---

## ⚙️ Commands Implemented
- Get Bootloader Version  
- Get Supported Commands  
- Get Chip ID  
- Get Read Protection Level  
- Jump to Address  
- Flash Erase  
- Memory Write  

## 🚧 Future Work
- Read/Write protection control
- Dual-bank & rollback protection  
- Memory read & OTP read handlers    
- OTA Firmware Updates

## 📂 Project Structure

- **STM32_Bootloader/**
  - **.metadata/** – STM32CubeIDE metadata files  
  - **Bootloader_STM32L496xx/** – Bootloader firmware source (STM32 project)  
  - **User_App_STM32L496xx/** – Example user application
  - **user_app.bin** – Precompiled user application binary  
  - **Docs/** – Documentation and Resources 
  - **STM32_Programmer_V1.py** – Host-side Python programmer script  
  - **README.md** – Project description  

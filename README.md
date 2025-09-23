# PLUTO PAYMENTS
A lightweight credit card system with hardware, backend and frontend implementations. Buit by [`Maksym`](https://github.com/Zar000), [`Johann`](https://github.com/hager3737) and [`Carl`](https://github.com/lafftale1999).

## Overview
### Hardware
- **Real-time OS**: FreeRTOS with tasks and queue management  
- **Networking**: Wi-Fi with connect/disconnect logic  
- **User Interface**: 16x2 LCD for live feedback  
- **Input**: 4x4 keypad for device interaction  
- **Card Reader**: RFID-RC522 for secure card data reading  
- **Security**:  
  - SHA-256 hashing for sensitive values  
  - HTTPS with mutual TLS (mTLS)  
  - HMAC tokens for integrity and replay-attack protection  

Link to project: https://github.com/lafftale1999/pluto_payments_hardware

### Backend
* **Networking**:
  - 8080 for requests through /api/*
  - 443 for confidential requests through /device/*
* **Session Based Login**: 30 minute sessions
* **DTOs**: For data sharing control
* **Security**:
  - mTLS connection on /device/*
  - HMAC control with device key
  - SHA256 hash for sensitive data

Link to project: https://github.com/lafftale1999/pluto_payments_backend

### Frontend overview


Link to project: https://github.com/lafftale1999/pluto_payments_frontend

## Dependencies
You can find all dependencies described in each submodule. Click on the module for information on how to download and build it.


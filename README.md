# PLUTO PAYMENTS
A lightweight credit card system with hardware, backend and frontend implementations. Built by [`Maksym`](https://github.com/Zar000), [`Johann`](https://github.com/hager3737) and [`Carl`](https://github.com/lafftale1999). For more information, please visit each individual module!

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
* Session-based login system using backend-issued cookies
* Secure API communication with the backend
* Account overview: see card, invoices, and account details
* Invoice details page with transaction history

Link to project: https://github.com/lafftale1999/pluto_payments_frontend

### Architecture
![System Architecture describing the whole ecosystem](resources/Pluto%20Payments%20Systemarkitektur.png)

### System Specification
We've included a System Specification in Swedish which describes our requirements specification, goal of the project, defending our module choices and which improvements that can be made. You can find the PDF here: [Link to PDF](resources/PlutoPayments.pdf)

## Clone project
To clone the project and all affected submodules use the command:
```sh
git clone --recurse-submodules https://github.com/lafftale1999/pluto_payments.git
```

## If you already cloned the project but didn't add the submodules, use this command:
```sh
git submodule update --init --recursive
```
## Dependencies
You can find all dependencies described in each submodule. Click on the module for information on how to download and build it.


# Parking Management System

This is a simple parking management project built for learning and practice. The application helps manage parking levels, parking spots, tickets, and basic payments using multiple backend services.

The main goal of this project is to understand how microservices work together, how APIs communicate, and how a frontend connects to backend services.

---

## What This Project Does

* Create parking levels and parking spots
* Show available parking spots
* Create a parking ticket when a vehicle enters
* Close the ticket when the vehicle exits
* Basic payment flow (mock / test)
* Simple admin and user screens

This project is not production ready and is mainly for learning and demo purposes.

---

## Tech Stack

**Backend**

* Java
* Spring Boot
* Spring Cloud (Gateway, Eureka, Config)
* PostgreSQL
* Docker

**Frontend**

* React
* Axios
* Bootstrap

---

## Project Structure

```
ML_Parking_Apk/
├── backend-service/
│   ├── api-gateway/
│   ├── config-server/
│   ├── discovery-server/
│   ├── parking-lot-service/
│   ├── ticketing-service/
│   ├── vehicle-service/
│   ├── payment-service/
│   ├── notification-service/
│   └── docker-compose.yml
├── frontend-service/
└── README.md
```

---

## Prerequisites

Make sure the following are installed:

* Java 17 or higher
* Node.js 18+
* Docker

---

## How to Run the Project

### Start Backend Services

```bash
cd backend-service
docker-compose up -d
```

Wait for a minute so that all services start.

You can open Eureka dashboard at:

```
http://localhost:8761
```

---

### Start Frontend

```bash
cd frontend-service
npm install
npm start
```

Open browser:

```
http://localhost:3000
```

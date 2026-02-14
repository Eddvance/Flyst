# Flyst

**A social platform built with microservices architecture.**

> ⚠️ This is a private project. This repository contains documentation only — no source code.

![Java](https://img.shields.io/badge/Java-17-orange?logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-green?logo=springboot)
![React Native](https://img.shields.io/badge/React%20Native-Mobile-blue?logo=react)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow)

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                            MOBILE APP                                    │
│                      React Native (iOS/Android)                          │
└───────────────────────────────┬─────────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                           API GATEWAY                                    │
└───────────┬───────────────────┼───────────────────┬─────────────────────┘
            │                   │                   │
            ▼                   ▼                   ▼
┌───────────────────┐ ┌───────────────────┐ ┌───────────────────┐
│     CERBERUS      │ │      FLYST        │ │     COLUMBA       │
│   Authentication  │ │       Core        │ │    Messaging      │
│                   │ │                   │ │                   │
│  • JWT tokens     │ │  • Publications   │ │  • Real-time      │
│  • User sessions  │ │  • User profiles  │ │  • Notifications  │
│  • Security       │ │  • Content mgmt   │ │  • Chat           │
└───────────────────┘ └───────────────────┘ └───────────────────┘
            │                   │                   │
            └───────────────────┼───────────────────┘
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                            WINYX                                         │
│                      Data Compression Service                            │
│                                                                          │
│              • Media optimization • Storage efficiency                   │
└─────────────────────────────────────────────────────────────────────────┘
                                │
                                ▼
┌─────────────────────────────────────────────────────────────────────────┐
│                          INFRASTRUCTURE                                  │
│                   PostgreSQL • Service Discovery                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 🧩 Microservices

| Service | Description | Status |
|---------|-------------|--------|
| **Flyst** | Core application — content management, user profiles | 🚧 In progress |
| **Cerberus** | Authentication service — JWT, session management | ✅ Developed |
| **Columba** | Messaging service — real-time communication | ✅ Developed |
| **Winyx** | Data compression — media optimization | 🚧 In progress |

---

## 🛠️ Tech Stack

**Backend**
- Java 17
- Spring Boot 3.x
- Spring Security + JWT
- PostgreSQL
- WebSocket (real-time messaging)

**Mobile**
- React Native (cross-platform iOS/Android)

**Infrastructure**
- Docker
- Service Discovery

---

## 🔐 Why Private?

This project contains proprietary business logic. This public repository serves as a portfolio showcase demonstrating:

- Microservices architecture design
- Service-to-service authentication
- Real-time messaging implementation
- Mobile app integration

---

## 👤 Author

**Edouard Leroy**  
Backend Developer | Java & Spring Boot  
[GitHub](https://github.com/Eddvance) • [LinkedIn](https://linkedin.com/in/edouard-leroy)

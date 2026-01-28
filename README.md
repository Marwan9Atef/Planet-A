# 🌍 Planet

**Planet** is a Flutter mobile application developed as a **teamwork project**, designed to provide a scalable and maintainable trip management system with a smooth and modern user experience.

The application follows **Clean Architecture**, a **feature-first structure**, and integrates mapping, authentication, caching, and backend services to simulate a real-world production-ready system.

---

## 📌 Project Description

Planet allows users to authenticate, browse available trips, view trip details, manage bookings, track trip history, and update personal profiles. Trip locations and routes are visualized using **OpenStreetMap**, enhancing the user experience with interactive maps.

The backend is built with **Laravel (PHP)** and exposes RESTful APIs for authentication, trip management, and user-related operations. To improve performance and reduce unnecessary API calls, the app implements a **local caching layer** using Hive.

The project emphasizes:

* Clean code
* Separation of concerns
* Scalability
* Team collaboration

---

## 👥 Team Members

This project was developed collaboratively by:

* **Marwan Atef** – Flutter Developer
  GitHub: [https://github.com/Marwan9Atef](https://github.com/Marwan9Atef)

* **Mohamed Yasser** – Flutter Developer
  GitHub: [https://github.com/midoyasser16204e](https://github.com/midoyasser16204e)

* **Abdalla Ahmed** – Flutter Developer
  GitHub: [https://github.com/Abdalla-Ahmed-Aly](https://github.com/Abdalla-Ahmed-Aly)

* **Mohamed Nasser** – Backend Developer
  GitHub: [https://github.com/MohamedNasser00](https://github.com/MohamedNasser00)

---

## ✨ Features Overview

* 🔐 Authentication (Phone & Google)
* 🧳 Trip Management
* 📍 Trip Location & Maps
* 🚗 Trip Details & Extra Trips
* ❌ Trip Cancellation
* 👤 User Profile Management
* 🕒 Trip History
* 💾 Local Caching & Offline Optimization

---

## 📸 Screenshots

### 🔐 Authentication

| Login                       | Register                       | OTP                       | Reset Password              |
| --------------------------- | ------------------------------ | ------------------------- | --------------------------- |
| ![](screens/auth/login.png) | ![](screens/auth/register.png) | ![](screens/auth/otp.png) | ![](screens/auth/reset.png) |

### 🧳 Trip Features

| Trip List                  | Trip Details                  | Extra Trip                  | Cancel Trip                  |
| -------------------------- | ----------------------------- | --------------------------- | ---------------------------- |
| ![](screens/trip/list.png) | ![](screens/trip/details.png) | ![](screens/trip/extra.png) | ![](screens/trip/cancel.png) |

### 👤 Profile

| Profile                          | Update Profile                          |
| -------------------------------- | --------------------------------------- |
| ![](screens/profile/profile.png) | ![](screens/profile/update_profile.png) |

### 🕒 Trip History

| History                          |
| -------------------------------- |
| ![](screens/history/history.png) |

---

## 🔐 Authentication Features

* Phone number & password login
* Google Sign-In
* OTP-based password reset
* Secure input validation
* Persistent login using cached data

---

## 🧳 Trip Features

* View available trips
* Trip details with seat selection
* Add extra trips
* Cancel booked trips
* View trip history
* Map-based trip visualization using OpenStreetMap

---

## 👤 Profile

* View user information
* Update profile details
* Display user-related trip data
* Cached profile data for fast loading

---

## 🛠️ Tech Stack

### 📱 Frontend (Mobile)

* **Flutter** (Dart)
* **State Management:** Bloc / Cubit
* **Networking:** Dio
* **Dependency Injection:** get_it / injectable
* **Architecture:** Clean Architecture
* **Maps:** OpenStreetMap (OSM)

---

### 💾 Caching & Local Storage

* **Hive** – Lightweight local database
* **Custom Cache Layer**

  * Cache user data
  * Cache trip data
  * Clear cache on logout
  * Improve performance & reduce API calls

---

### 🖥 Backend

* **PHP**
* **Laravel Framework**
* **RESTful APIs**
* **Authentication & Authorization**

---

## 🧱 Architecture Overview

The project follows a **Feature-Based Clean Architecture** approach.
Each feature is isolated and divided into **Data**, **Domain**, and **Presentation** layers.

---

### 📁 Feature Structure

```
feature_name/
│
├── data/
│   ├── datasources/        # Remote / local data sources
│   ├── models/             # API & cache models
│   ├── mappers/            # Model ↔ Entity conversion
│   └── repositories/       # Repository implementations
│
├── domain/
│   ├── entities/           # Business entities
│   ├── repositories/       # Repository abstractions
│   └── usecases/           # Business logic
│
├── presentation/
│   ├── cubit/              # State management
│   ├── screens/            # UI screens
│   └── widgets/            # Feature widgets
```

---

### 🔁 Layer Responsibilities

#### 🗄 Data Layer

* Handles API requests and caching
* Maps raw data into domain entities
* Implements repository contracts

#### 🧠 Domain Layer

* Pure business logic
* Independent from Flutter & external libraries
* Contains use cases and entities

#### 🎨 Presentation Layer

* UI & user interaction
* State management using Cubit
* Screens and reusable widgets

---

## 📂 Core Module

The `core` module contains shared functionality across the app:

```
core/
├── cache/          # Local caching & logout handling
├── di/             # Dependency injection setup
├── constants/      # App-wide constants
├── services/       # Shared services (API, helpers)
├── utils/          # Utility functions
├── theme/          # App theming
└── widgets/        # Reusable UI components
```

---

## 📂 Main Project Structure

```
lib/
│
├── core/
├── features/
│   ├── auth/
│   ├── trip/
│   ├── trip-detail/
│   ├── extra-trip/
│   ├── cancel-trip/
│   ├── history/
│   ├── profile/
│   └── location/
│
└── main.dart
```

---


## 🚧 Future Enhancements

* 📍 Real-time trip tracking
* 💳 Online payment integration
* 🔔 Push notifications
* 🌍 Multi-language support


---

## ⭐ Acknowledgment

 Thanks to all team members for their collaboration and effort in building this project.

* Special thanks to Youssef Salah For his Support 

  GitHub: [https://github.com/YousefSalah1](https://github.com/YousefSalah1)

If you find this project useful, please consider giving it a **star ⭐**.





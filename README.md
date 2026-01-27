# 🌍 Planet

**Planet** is a Flutter mobile application developed as a **teamwork project**, focusing on clean architecture, scalability, and a smooth user experience. The app provides authentication, trip management, and user profile features with a modern and user-friendly UI.

---

## 👥 Team Members

This project was developed collaboratively by:

* **Marwan Atef** – Flutter Developer
  GitHub: [https://github.com/Marwan9Atef](https://github.com/Marwan9Atef)

* **Mohamed Yasser** – Flutter Developer 
  GitHub: [https://github.com/midoyasser16204e](https://github.com/midoyasser16204)

* **Abdalla Ahmed** – Flutter Developer
  GitHub: [https://github.com/Abdalla-Ahmed-Aly](https://github.com/Abdalla-Ahmed-Aly)
  
* **Mohamed Nasser** – BackEnd Developer
  GitHub: [https://github.com/MohamedNasser00](https://github.com/MohamedNasser00)



---

## ✨ Features Overview

* 🔐 Authentication (Phone & Google)
* 🧳 Trip Management
* 🚗 Trip Details & Extra Trips
* 👤 User Profile
* 🕒 Trip History

---

## 🔐 Authentication Features

### 📸 Screens

> Add authentication-related screenshots here

| Login                            | Register                               | OTP                          | Reset Password                   |
| -------------------------------- | -------------------------------------- | ---------------------------- | -------------------------------- |
| ![Login](screens/auth/login.png) | ![Register](screens/auth/register.png) | ![OTP](screens/auth/otp.png) | ![Reset](screens/auth/reset.png) |

### Login

* Login using **phone number + password**
* Login with **Google** using `google_sign_in` package
* Secure and validated input fields

### Register

* Register using phone number and password
* Basic user information setup

### OTP Flow

* Send OTP to **email**
* Verify OTP code
* Reset password using OTP verification

---

## 🧳 Trip Features

### 📸 Screens

> Add trip-related screenshots here

| Trip List                       | Trip Details                         | Extra Trip                       | Cancel Trip                        |
| ------------------------------- | ------------------------------------ | -------------------------------- | ---------------------------------- |
| ![Trips](screens/trip/list.png) | ![Details](screens/trip/details.png) | ![Extra](screens/trip/extra.png) | ![Cancel](screens/trip/cancel.png) |

### Trip List

* Display available trips
* Show trip source, destination, time, and available seats

### Trip Details

* View full trip information
* Seat selection interface
* Payment action

### Extra Trip

* Add an extra trip from trip details

### Cancel Trip

* Allow user to cancel an existing trip
* Update trip status accordingly

---

## 👤 Profile

### 📸 Screens

> Add profile-related screenshots here

| Profile                                 | Update Profile                                        |
| --------------------------------------- | ----------------------------------------------------- |
| ![Profile](screens/profile/profile.png) | ![Update Profile](screens/profile/update_profile.png) |

* Display user personal information
* Update profile information (name, phone, etc.)
* View user-related trip data



---

## 🕒 Trip History

### 📸 Screens

> Add trip history screenshots here

| History                                 |
| --------------------------------------- |
| ![History](screens/history/history.png) |

* Display history of all previous trips
* Each trip shown in a card format
* Clear and readable timeline

---

## 🛠️ Tech Stack

* **Flutter** (Dart)
* **State Management:** Bloc / Cubit
* **Networking:** Dio
* **Dependency Injection:** get_it / injectable
* **Authentication:** Google Sign-In
* **Architecture:** Clean Architecture (Data / Domain / Presentation)

---

## 📂 Project Structure

```
lib/
│── core/
│   ├── constants/
│   ├── errors/
│   ├── helpers/
│   └── widgets/
│
│── features/
│   ├── auth/
│   ├── trip/
│   ├── profile/
│   └── history/
│
│── main.dart
```

---

## 🚧 Future Enhancements

* [ ] Dark mode support
* [ ] Better animations
* [ ] Improved error handling
* [ ] More unit & integration tests

---

## ⭐ Acknowledgment

Special thanks to all team members who contributed to this project.

If you like this project, don’t forget to ⭐ the repository!

---



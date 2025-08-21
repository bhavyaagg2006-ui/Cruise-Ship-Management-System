# Cruise Ship Management System

A comprehensive web-based system to manage onboard services on a cruise ship.  
This project supports multiple roles with role-based features and Firebase-backed authentication & data storage.

---

## 🎯 Objectives
- Provide a simple, attractive UI for voyagers to order and book services.
- Enable admins/managers to manage items, sessions, and monitor operations.
- Use Firebase Authentication + Firestore for fast evaluation and easy setup.

---

## 👥 User Roles

- **Voyager** – End-user for ordering and booking services.
- **Admin** – Manages entire system, items, sessions, users.
- **Manager** – Oversees daily operations; can approve/monitor orders & bookings.
- **Head-Cook** – Manages catering items/menu and updates order statuses.
- **Supervisor** – Monitors services and coordinates between departments.

---

## ✨ Features

### Voyager
- Signup & Login (Firebase Auth)
- Catering Item Ordering
- Stationery Item Ordering
- Movie/Resort Ticket Booking
- Beauty Salon Booking
- Fitness Center Booking
- Party Hall Booking
- Light/Dark Theme Toggle

### Admin
- Add/Edit/Delete Items (Catering, Stationery, Fitness Sessions,Party Hall,Resort)
- Manage Menu/Inventory
- Register Voyagers / Manage Users
- View all orders & update status

### Manager
- View all orders & bookings
- Approve/Reject/Update statuses
- View service analytics (basic)

### Head-Cook
- Add/Edit catering items (name, price, image)
- Update catering order status (e.g., Received → Preparing → Delivered)

### Supervisor
- Monitor orders/bookings across departments
- View issue logs / service coordination

---

## 🧰 Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend (BaaS):** Firebase Authentication & Firestore
- **Hosting:** Local / Firebase Hosting
- **VCS:** Git & GitHub

---

## 📁 Project Structure 
**root**/
  index.html
  signup.html
  login.html
/
**dashboards**/
  voyager.html
  admin.html
  manager.html
  headcook.html
  supervisor.html
/
**features**/
  catering.html
  stationery.html
  resort.html
  salon.html
  fitness.html
  partyhall.html
/
**javascript**/
  firebase-config.js
  auth.js
  voyager.js
  admin.js
  manager.js
  headcook.js
  supervisor.js
/
**css**/
  styles.css
/
## 🔐 Firebase Setup

### 1) Create Firebase project
- Go to Firebase Console → Create Project.
- Enable **Authentication** → **Sign-in method** → **Email/Password**.
- Enable **Firestore Database** → Start in **Test mode** .

### 2) Firebase configuration
```javascript
const firebaseConfig = {
  apiKey: "AIzaSyD0cA756dZeVEbR4Vqovsh5p74niMxNT3w",
  authDomain: "cruise-ship-management-s-98138.firebaseapp.com",
  projectId: "cruise-ship-management-s-98138",
  storageBucket: "cruise-ship-management-s-98138.firebasestorage.app",
  messagingSenderId: "401246402444",
  appId: "1:401246402444:web:dd8a21a7e144e90d3788a9",
  measurementId: "G-29GKF5F9SS"
};

// Initialize Firebase
firebase.initializeApp(firebaseConfig);
const auth = firebase.auth();
const db = firebase.firestore();

### 3) Firebase Rules
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /{document=**} {
      allow read, write: if true;
    }
  }
}```
---
## 🚀 Setup & Run

Follow these steps to set up and run the Cruise Ship Management System project on your local machine:

### 1. Clone the Repository
```bash
git clone https://github.com/bhavyaagg2006-ui/cruise-ship-management.git
cd cruise-ship-management
---

## 📸 Screenshots

## Login Page
![Login Screenshot](https://raw.githubusercontent.com/bhavyaagg2006-ui/Cruise-Ship-Management-System/main/screenshots/login.png)

## Signup Page
![Signup Screenshot](https://raw.githubusercontent.com/bhavyaagg2006-ui/Cruise-Ship-Management-System/main/screenshots/signup.png)



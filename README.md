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

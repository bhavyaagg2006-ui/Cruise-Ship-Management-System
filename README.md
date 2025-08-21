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
 -index.html
 -signup.html
 -login.html
/
**dashboards**/
  -voyager.html
  -admin.html
  -manager.html
  -headcook.html
  -supervisor.html
/
**features**/
  -catering.html
  -stationery.html
  -resort.html
  -salon.html
  -fitness.html
  -partyhall.html
/
**javascript**/
  -firebase-config.js
  -auth.js
  -voyager.js
  -admin.js
  -manager.js
  -headcook.js
  -supervisor.js
/
**css**/
  -styles.css
/

## Setup & Installation

1. **Clone the repository:**  
```bash
git clone <https://github.com/bhavyaagg2006-ui/Cruise-Ship-Management-System.git>
```

2. **Open the project folder in VS Code (or any code editor).**

3. **Create a Firebase project:**
-Go to Firebase Console
-Click Add Project → Follow steps to create a new project

4. **Enable Authentication:**
-Navigate to Authentication → Sign-in method
-Enable Email/Password sign-in

5. **Create Firestore Database:**
-Go to Firestore Database → Create Database
-Start in Test Mode
-Create collections

6. **Add Firebase config in your HTML files:**

**// Firebase configuration**
```bash
const firebaseConfig = {
  apiKey: "AIzaSyD0cA756dZeVEbR4Vqovsh5p74niMxNT3w",
  authDomain: "cruise-ship-management-s-98138.firebaseapp.com",
  projectId: "cruise-ship-management-s-98138",
  storageBucket: "cruise-ship-management-s-98138.firebasestorage.app",
  messagingSenderId: "401246402444",
  appId: "1:401246402444:web:dd8a21a7e144e90d3788a9",
  measurementId: "G-29GKF5F9SS"
};
```
**// Initialize Firebase**
```bash
firebase.initializeApp(firebaseConfig);
```
7. **Open index.html or login.html in your browser to test the application.**

---

## 📸 Screenshots

### 1. Signup Page
![Signup page](screenshots/signup.png)

### 2. Login Page
![login page](screenshots/login.png)

### 3. Voyager Dashboard
![Voyager Dashboard](screenshots/voyager_dashboard.png)

### 4. Order Catering
![Order Catering](screenshots/order_catering.png)

### 5. Order Stationery
![Order Stationery](screenshots/order_stationery.png)

### 6. Book Fitness
![Book Fitness](screenshots/fitness_booking.png)

### 7. Book Salon
![Book Salon](screenshots/salon_booking.png)

### 8. Book Resort 
![Book Resort](screenshots/resort_booking.png)

### 9. Book Party Hall 
![Book Party Hall](screenshots/partyhall_booking.png)

### 10. Admin Dashboard
![Admin Dashboard](screenshots/admin_dashboard.png)

### 11. Add New Items
![Add New Items](screenshots/add_items.png)

### 12. Edit/Delete Items
![Edit/Delete Items](screenshots/edit_delete_items.png)

### 13. Maintain Menu Items
![Maintain Menu Items](screenshots/menu_items.png)

### 14. Voyager Registration
![Voyager Registration](screenshots/voyager_registration.png)

### 15. Manager Dashboard
![Manager Dashboard](screenshots/manager_dashboard.png)

### 16. View Booked Resort
![View Booked Resort](screenshots/view_resort.png)

### 17. View Booked Salon
![View Booked Saloon](screenshots/view_salon.png)

### 18. View Booked Fitness
![View Booked Fitness](screenshots/view_fitness.png)

### 19. View Booked Party Hall
![View Booked Party Hall](screenshots/view_partyhall.png)

### 20. Head-Cook Dashboard
![Head-Cook Dashboard](screenshots/headcook_dashboard.png)

### 21. View Ordered Catering
![View Ordered Catering](screenshots/view_catering.png)

### 22. Supervisor Dashboard
![Supervisor Dashboard](screenshots/supervisor_dashboard.png)

### 23. View Booked Stationery
![View Booked Stationery](screenshots/view_stationery.png)

---

## 👤 Usage
1. **Voyager (Passenger):**  
   - Sign up with your email and password  
   - Log in to access the **Voyager Dashboard**  
   - Perform the following actions:  
     - Order catering items 🍽️  
     - Order stationery items 🖊️  
     - Book resort/movie tickets 🎬  
     - Book beauty salon 💇‍♀️  
     - Book fitness center 🏋️‍♂️  
     - Book party hall 🎉   

2. **Admin:**  
   - Log in with admin credentials  
   - Add/Edit/Delete items (catering, fitness sessions, etc.)  
   - Manage voyager registrations  
   - Maintain menus and services  

3. **Future Staff Roles:**  
   - Manager, Head Cook, Supervisor modules will have dedicated dashboards  
   - Access will be based on role-based login and permissions

---

## 🛂 Contributing

We welcome contributions to improve this project! Follow these steps:

1. **Fork this repository**  
   - Click the **Fork** button on the top-right of this repo.

2. **Clone your forked repository:**  
```bash
git clone https://github.com/bhavyaagg2006-ui/Cruise-Ship-Management-System.git
```

3. **Create a new branch:**
```bash
git checkout -b feature-name
```

4. **Make your changes:**
   -Add new features.
   -Fix bugs.
   -Enhance the design.

6. **Commit your changes:**
```bash
git add .
git commit -m "Added feature: <short-description>"
```

6. **Push to your branch:**
```bash
git push origin feature-name
```

7. **Create a Pull Request:**
   -Go to your forked repository on GitHub.
   -Click Compare & Pull Request.
   -Add a clear description and submit it for review.

---

## 🪪 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

## 🔮 Future Enhancements

- Manager, Head Cook, Supervisor modules  
- Real-time notifications  
- Payment integration  

---

## 🏆 Credits

- Developed by **Bhavya Aggarwal**  
- Guided step-by-step using **OpenAI GPT-5**  

---

## 📞 Contact

For queries or suggestions:  
- GitHub: [bhavyaagg2006-ui]( https://github.com/bhavyaagg2006-ui)  
- Email: bhavyaagg2006@gmail.com




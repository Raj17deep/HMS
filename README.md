# 🏨 Rest Easy – Hotel Management System

A **Hotel Management System (HMS)** built using **Node.js, Express, and HTML/CSS/JS front-end**, designed to streamline hotel operations such as room bookings, staff management, payments, and dashboards for administrators.

This project provides a functional prototype of a hotel’s digital management system with multiple interfaces for **Admins, Staff, Receptionists, and Guests**.

---

## 📂 Project Structure

```
raj17deep-hms/
│── aboutus.html           # About Us page
│── admin.html             # Admin login portal
│── bookingpage.html       # Admin room booking management
│── confirm.html           # Booking confirmation page
│── contactus.html         # Contact Us page
│── dash.html              # Basic Admin dashboard (static)
│── dashboard.html         # Interactive Admin dashboard with charts
│── features.html          # System features overview
│── findaccount.html       # Account recovery page
│── index.html             # Landing page (Rest Easy Hotel)
│── mainpage.html          # Alternate main page
│── package.json           # Node.js dependencies and scripts
│── payment.html           # Payment handling page
│── receptionist-login.html# Receptionist login
│── register.html          # User registration
│── render.yaml            # Render.com deployment config
│── rooms.html             # Rooms display (static)
│── rooms2.html            # Rooms management (admin)
│── server.js              # Backend server (Express + APIs)
│── signup.html            # Signup form
│── staff.html             # Staff management
│── staffattendance.html   # Staff attendance tracking
│── stafflogin.html        # Staff login page
│── style.css              # Stylesheet (global)
│── style1.css - style4.css# Page-specific styles
│── submit.html            # Contact form submission response
```

---

## 🚀 Features

### 👤 **Guest/User Features**

* Browse rooms and hotel details.
* Register and log in as a guest.
* Submit booking requests.
* Receive booking confirmation.
* Contact the hotel via the contact form.

### 🛎️ **Receptionist/Staff Features**

* Staff login & attendance tracking.
* Manage guest check-ins/check-outs.
* View assigned tasks.

### 🛠️ **Admin Features**

* Admin login dashboard.
* **Booking Management:** View, confirm, edit, or delete reservations.
* **Room Management:** Add and manage available rooms.
* **Staff Management:** Track staff info and attendance.
* **Analytics Dashboard:**

  * Room occupancy (Chart.js doughnut chart).
  * Revenue trends (Chart.js bar chart).
* Export reservations to Excel.
* Generate PDF invoices for guests (using **jsPDF**).

---

## 🖥️ Tech Stack

### **Frontend**

* HTML5, CSS3, JavaScript (Vanilla)
* FontAwesome icons, Google Fonts
* Chart.js (Admin dashboard graphs)

### **Backend**

* **Node.js + Express.js** (via `server.js`)
* REST APIs for reservations and staff management

### **Utilities**

* **jsPDF** & **jspdf-autotable** → PDF Invoice generation
* **Excel Export** via backend endpoint
* **Render.com Deployment** → `render.yaml`

---

## ⚙️ Setup & Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/raj17deep-hms.git
cd raj17deep-hms
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Run the Server

```bash
node server.js
```

Server will start at: **[http://localhost:5502/](http://localhost:5502/)**

### 4️⃣ Access Frontend

Open `index.html` in your browser OR run the app via Render/Node server.

---

## 🌐 API Endpoints

The backend (`server.js`) exposes APIs for managing reservations and staff.

* `GET /api/reservations` → Fetch all reservations
* `GET /api/reservations/:id` → Fetch a single reservation
* `POST /api/reservations` → Create a reservation
* `PUT /api/reservations/:id` → Update reservation details
* `PATCH /api/reservations/:id` → Update reservation status
* `DELETE /api/reservations/:id` → Delete reservation
* `GET /api/export-reservations` → Export all reservations to Excel
* `GET /api/dashboard-stats` → Fetch statistics for dashboard

---

## 📊 Screens & Pages

* **Landing Page (`index.html`)** → Welcome page for guests
* **About Us (`aboutus.html`)** → Mission, vision & hotel details
* **Contact Us (`contactus.html`)** → Hotel contact info & form
* **Admin Login (`admin.html`)** → Admin, staff, and receptionist login options
* **Dashboard (`dashboard.html`)** → Admin dashboard with live charts
* **Booking Management (`bookingpage.html`)** → Full CRUD on bookings
* **Staff Management (`staff.html`)** → Manage hotel staff
* **Confirm Page (`confirm.html`)** → Displays booking confirmation

---

## ☁️ Deployment

This project includes **`render.yaml`**, which allows deployment on [Render.com](https://render.com).
To deploy:

1. Push repo to GitHub.
2. Connect to Render.com.
3. Render will auto-detect `node server.js` as the start command.

---

## 👥 Authors

* **Rajdeep Choudhury** – Project Developer
* Hotel project prototype for educational/demo purposes.

---

## 📌 Future Improvements

* Add database integration (MongoDB/MySQL) instead of mock/local storage.
* Implement JWT-based authentication.
* Add real payment gateway (Razorpay/Stripe).
* Enable bulk booking imports.

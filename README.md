# 📸 Face Recognition Attendance System

A mobile-first AI-powered attendance system that uses **face recognition**, **live detection**, and **GPS validation** to log user attendance in real-time—ensuring authenticity and location-bound check-ins.

## 🌟 Features

### 📱 Mobile App (Expo)
- **Face Recognition** with live camera feed
- **Liveness Detection** to prevent spoofing (blink/head movement)
- **GPS Location Logging** to validate user is within office premises
- **One-Click Check-In/Out**
- **Offline Mode** with sync support

### 🛠️ Backend (Express.js)
- **RESTful API** for user, attendance, and admin features
- **JWT Authentication** and Role-based Access (Admin, Employee)
- **MongoDB** or **PostgreSQL** integration for storage
- **Image/Embedding Processing** and Attendance Logging
- **Geofencing Support** (configurable)

### 🖥️ Admin Dashboard
- Create/Edit/Delete User Profiles with face data
- View and filter attendance logs by date/user
- Export reports in CSV or PDF format
- User leave management and manual override
- Audit logs of user activities

---

## 🧱 Tech Stack

| Layer       | Technology              |
|------------|--------------------------|
| Frontend    | Expo (React Native), Expo Camera, Location API |
| Backend     | Node.js, Express.js      |
| Database    | MongoDB / PostgreSQL     |
| Face Recognition | TensorFlow.js, face-api.js, or native ML Kit |
| Liveness Detection | Mediapipe or blink/head movement tracking |
| Hosting     | Render, Railway, or VPS |

---

## 🔐 Security & Privacy
- Face data processed using secure embeddings (not stored as raw images)
- End-to-end HTTPS communication
- GPS anti-spoof checks (basic)
- Admin-only access to sensitive logs and reports

---

## 🧩 Planned Features
- Push Notifications (reminders, status)
- Geofencing via polygonal boundaries
- Native ML Kit integration (optional if ejected from Expo)
- Biometric fallback (Face ID / Fingerprint)
- Slack/Email notifications for check-ins

---

## ⚙️ Project Setup

### 🔧 Frontend (Expo)
cd mobile-app
npm install
npx expo start

### 🔧 Backend (Express)
cd backend
npm install
npm run dev

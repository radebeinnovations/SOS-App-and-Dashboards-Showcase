# 🚨 SOS South Africa

> **SOS South Africa** is a full emergency response and community safety platform built for South African communities. Citizens can trigger SOS alerts, report incidents, and view a live community crime map — while responders and administrators manage everything from two dedicated web dashboards. Built with **React Native (Expo)** for mobile and **React** for both dashboards, powered by **Firebase** on the backend.

---

## 💡 What It Does

SOS South Africa has three parts working together in real time:

**📱 Mobile App — for citizens**
Open the app, hit the SOS button, describe your emergency, and your location is instantly broadcast to responders. You can also access the Community Crime Map to view and report incidents in your area — but only once you're signed up.

**🖥️ Responder Dashboard — for emergency responders**
A live dashboard showing all active SOS alerts, incident locations on a map, and a full activity feed. Responders can track, manage, and resolve incoming alerts in real time.

**🖥️ Admin Dashboard — for administrators**
A higher-level overview of all system activity — incidents, users, alerts, and community reports — giving administrators full visibility and control over the platform.

---

## 📸 Screenshots

### 📱 Mobile App

#### Welcome & SOS Alert

<img src="https://github.com/user-attachments/assets/82ce6bc2-f3bf-46b5-97f0-c39802ad335b" width="300" alt="SOS Alert Welcome Screen" />

---

#### Describe Your Emergency

<img src="https://github.com/user-attachments/assets/a11b1c00-4d0e-40c5-aa2a-d72143d4c948" width="300" alt="Describe Your Emergency" />

---

#### Live Location Map & Emergency Confirmation

<p float="left">
  <img src="https://github.com/user-attachments/assets/060c8c5e-f769-4093-8868-d167edc7e0fe" width="300" alt="Map with Location Pin" />
  <img src="https://github.com/user-attachments/assets/fdd103a9-7d3d-4cd5-abf5-d751fd46f19c" width="300" alt="Emergency Popup on Map" />
  <img src="https://github.com/user-attachments/assets/dabf746f-45c0-4681-a63b-e20662f61e7b" width="300" alt="Map with Route" />
</p>

---

#### Community Crime Map
> Sign-up required to access the Community Crime Map and alerts

<p float="left">
  <img src="https://github.com/user-attachments/assets/f457ae3b-f9dc-487c-a713-ef4d9f504912" width="300" alt="Community Crime Map" />
  <img src="https://github.com/user-attachments/assets/6ea733e0-c3a1-42f1-b834-4577c7a6a22a" width="300" alt="Report Incident Form" />
  <img src="https://github.com/user-attachments/assets/38cdbaec-749a-4688-ace1-f5f73470b7c5" width="300" alt="Community Map with Incident Radius" />
</p>

---

#### Access Restricted
> Users must be signed up to access the Community Crime Map alerts

<img src="https://github.com/user-attachments/assets/e94edaa0-8fc9-4efd-9bca-2e6182fb5fbc" width="300" alt="Access Restricted Screen" />

---

### 🖥️ Responder Dashboard

> Live dashboard for emergency responders — tracks all active SOS alerts, incident locations, and activity in real time

<img src="https://github.com/user-attachments/assets/e1b8fe01-636d-4a15-881f-db3456a88850" width="100%" alt="Responder Dashboard Overview" />

<img src="https://github.com/user-attachments/assets/31a677a9-d233-431f-a441-038ccd1c5cc4" width="100%" alt="Responder Dashboard Incidents List" />

<img src="https://github.com/user-attachments/assets/4d672327-9547-48a0-ae31-97b8f00fc98b" width="100%" alt="Responder Dashboard Map View" />

---

### 🖥️ Admin Dashboard

> High-level system overview for administrators — full visibility over all alerts, users, incidents, and community reports

<img src="https://github.com/user-attachments/assets/50697773-0bde-417f-945b-32a7a3fcf6cc" width="100%" alt="Admin Dashboard Overview" />

<img src="https://github.com/user-attachments/assets/1dab2e9e-fef8-48cd-9433-bafd453de263" width="100%" alt="Admin Dashboard Incidents" />

<img src="https://github.com/user-attachments/assets/b97c489e-9bbc-46b8-9a27-6dadb37fa8f1" width="100%" alt="Admin Dashboard Map View" />

<img src="https://github.com/user-attachments/assets/96161973-9ecc-490d-aa84-8468b678eca6" width="100%" alt="Admin Dashboard Additional View" />

---

## ⚙️ How It Works

```
Citizen triggers SOS on mobile app
        ↓
Firebase logs alert with live GPS location
        ↓
Responder Dashboard receives alert in real time
        ↓
Responder tracks, manages, and resolves the alert
        ↓
Admin Dashboard maintains full oversight of all activity
```

---

## 🛠️ Built With

| Layer | Technology |
|---|---|
| Mobile App | React Native + Expo |
| Responder Dashboard | React |
| Admin Dashboard | React |
| Backend & Database | Firebase Firestore |
| Authentication | Firebase Auth |
| Real-time updates | Firebase Realtime Listeners |
| Maps | Google Maps API |

---

## 🚀 Running It Locally

You'll need **Node.js (v18+)**, **Expo CLI**, and a **Firebase project** with Firestore and Authentication enabled.

### Mobile App

**1. Clone the repo:**
```bash
git clone https://github.com/radebeinnovations/SOS-App-and-Dashboards-Showcase.git
cd SOS-App-and-Dashboards-Showcase
npm install
```

**2. Add your Firebase credentials:**
```js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

**3. Start the app:**
```bash
npx expo start
```
Scan the QR code with **Expo Go** on your phone.

---

### Responder Dashboard

```bash
cd ResponderDashboard
npm install
npm start
```
Opens at `http://localhost:3000`

---

### Admin Dashboard

```bash
cd AdminDashboard
npm install
npm start
```
Opens at `http://localhost:3001`

---

## 📁 Project Layout

```
SOS-App-and-Dashboards-Showcase/
├── SOSApp/                ← React Native mobile app
├── ResponderDashboard/    ← Live responder web dashboard
├── AdminDashboard/        ← Admin oversight web dashboard
└── README.md
```

---

## 📝 Notes

- The **Community Crime Map** on the mobile app requires users to be signed up and authenticated before accessing alerts and incident reporting.
- Both dashboards require admin/responder credentials via Firebase Auth.
- If setting up fresh, create your admin users in the Firebase console first.

---

> Built by **Radebe Innovations** 🚀

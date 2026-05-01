# 🚨 SOS South Africa

> **SOS South Africa** is a full emergency response and community safety platform built for South African communities. Citizens can trigger SOS alerts, report incidents, and view a live community crime map — while call centre operators and responders manage everything from two dedicated web dashboards. Built with **React Native (Expo)** for mobile and **React** for both dashboards, powered by **Firebase** on the backend.

---

## 💡 What It Does

SOS South Africa has three parts working together in real time:

**📱 Mobile App — for citizens**
Open the app, hit SOS, describe your emergency, and the system instantly locates the nearest emergency station to you. The responder is dispatched and you can track them live. If you're too shaken to call, the app automatically shows a call option 10 seconds after your request. Citizens can also access the Community Crime Map to view and report incidents — registration required to keep the community safe from anonymous actors.

**🖥️ Call Centre Dashboard — for operators**
A live overview of all active SOS alerts, incident locations on a map, and a full activity feed. Call centre operators can see every emergency as it comes in, track its status, and coordinate response in real time.

**🖥️ Responder Dashboard — for police & medics**
Responders log in, see incoming emergencies assigned to them, accept the call, and Google Maps guides them directly to the scene.

---

## 📸 Screenshots

### 📱 Mobile App — SOS Emergency Flow

#### 1. Welcome & Get Started

<img src="https://github.com/user-attachments/assets/82ce6bc2-f3bf-46b5-97f0-c39802ad335b" width="300" alt="SOS Alert Welcome Screen" />

---

#### 2. Describe Your Emergency
> Select your emergency type and send the alert

<img src="https://github.com/user-attachments/assets/a11b1c00-4d0e-40c5-aa2a-d72143d4c948" width="300" alt="Describe Your Emergency" />

---

#### 3. Locating Nearest Emergency Station
> The app finds the closest available station to your GPS location

<img src="https://github.com/user-attachments/assets/060c8c5e-f769-4093-8868-d167edc7e0fe" width="300" alt="Locating Nearest Emergency Station" />

---

#### 4. Station Located & Responder Dispatched
> Confirmation that a station has been found and help is on the way

<img src="https://github.com/user-attachments/assets/fdd103a9-7d3d-4cd5-abf5-d751fd46f19c" width="300" alt="Emergency Station Located" />

---

#### 5. Live Route Tracking + Call Option
> Track the responder live — if you're too shaken to act, the call option automatically appears after 10 seconds

<p float="left">
  <img src="https://github.com/user-attachments/assets/dabf746f-45c0-4681-a63b-e20662f61e7b" width="300" alt="Route Tracking with Alert Security and Call Police" />
  <img src="https://github.com/user-attachments/assets/f457ae3b-f9dc-487c-a713-ef4d9f504912" width="300" alt="Call Option Appears After 10 Seconds" />
</p>

---

### 📱 Mobile App — Community Crime Map

> Accessible from the Alerts button on the main page. Citizens can view reported incidents and report new ones. If 3 or more crimes are reported in the same area, that area is automatically flagged as a hotspot with a red circle.

#### Community Crime Map

<img src="https://github.com/user-attachments/assets/6ea733e0-c3a1-42f1-b834-4577c7a6a22a" width="300" alt="Community Crime Map" />

---

#### Report an Incident

<img src="https://github.com/user-attachments/assets/e94edaa0-8fc9-4efd-9bca-2e6182fb5fbc" width="300" alt="Report Incident Form" />

---

#### Crime Hotspot — 3+ Reports in One Area
> Areas with 3 or more reports are automatically marked with a red hotspot circle

<img src="https://github.com/user-attachments/assets/38cdbaec-749a-4688-ace1-f5f73470b7c5" width="300" alt="Crime Hotspot Red Circle" />

---

#### 🔒 Access Restricted
> You must complete your profile before reporting crimes — this keeps the community safe from anonymous actors

<img src="https://github.com/user-attachments/assets/e1b8fe01-636d-4a15-881f-db3456a88850" width="300" alt="Access Restricted Screen" />

---

### 🖥️ Call Centre Dashboard

> Operators see every active SOS alert, track incidents on a live map, and coordinate emergency response in real time

<img src="https://github.com/user-attachments/assets/31a677a9-d233-431f-a441-038ccd1c5cc4" width="100%" alt="Call Centre Dashboard" />

---

### 🖥️ Responder Dashboard

> Police and medics log in, see emergencies assigned to them, accept the call, and are guided to the scene via Google Maps

<img src="https://github.com/user-attachments/assets/4d672327-9547-48a0-ae31-97b8f00fc98b" width="100%" alt="Responder Dashboard Overview" />

<img src="https://github.com/user-attachments/assets/50697773-0bde-417f-945b-32a7a3fcf6cc" width="100%" alt="Responder Dashboard Incidents" />

<img src="https://github.com/user-attachments/assets/1dab2e9e-fef8-48cd-9433-bafd453de263" width="100%" alt="Responder Dashboard Map View" />

<img src="https://github.com/user-attachments/assets/b97c489e-9bbc-46b8-9a27-6dadb37fa8f1" width="100%" alt="Responder Dashboard Route" />

<img src="https://github.com/user-attachments/assets/96161973-9ecc-490d-aa84-8468b678eca6" width="100%" alt="Responder Dashboard Additional View" />

---

## ⚙️ How It Works

```
Citizen triggers SOS on the mobile app
              ↓
System locates the nearest emergency station via GPS
              ↓
Responder is dispatched — citizen tracks them live
              ↓
Call option auto-appears after 10 seconds if citizen hasn't called
              ↓
Call Centre Dashboard monitors everything in real time
              ↓
Responder Dashboard guides police/medics to the scene
```

---

## 🛠️ Built With

| Layer | Technology |
|---|---|
| Mobile App | React Native + Expo |
| Call Centre Dashboard | React |
| Responder Dashboard | React |
| Backend & Database | Firebase Firestore |
| Authentication | Firebase Auth |
| Real-time sync | Firebase Realtime Listeners |
| Maps & Routing | Google Maps API |

---

## 🚀 Running It Locally

You'll need **Node.js (v18+)**, **Expo CLI**, and a **Firebase project** with Firestore and Authentication enabled.

### 📱 Mobile App

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

### 🖥️ Call Centre Dashboard

```bash
cd CallCentreDashboard
npm install
npm start
```
Opens at `http://localhost:3000`

---

### 🖥️ Responder Dashboard

```bash
cd ResponderDashboard
npm install
npm start
```
Opens at `http://localhost:3001`

---

## 📁 Project Layout

```
SOS-App-and-Dashboards-Showcase/
├── SOSApp/                  ← React Native mobile app
├── CallCentreDashboard/     ← Live call centre web dashboard
├── ResponderDashboard/      ← Responder web dashboard
└── README.md
```

---

## 📝 Notes

- The **Community Crime Map** requires profile verification before reporting incidents — this protects the community from anonymous actors.
- Areas with **3 or more reports** in the same location are automatically flagged as crime hotspots.
- The **call option** on the SOS tracking screen appears automatically after 10 seconds in case the citizen is too shaken to act.
- Both dashboards require credentials via Firebase Auth — create your users in the Firebase console first.
- Never commit your real `.env` file or Firebase credentials to GitHub — always add `.env` to your `.gitignore`.

---

> Built by **Radebe Innovations** 🚀

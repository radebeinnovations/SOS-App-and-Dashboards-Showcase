# 🚨 SOS South Africa
 
> **SOS South Africa** is a full emergency response and community safety platform built for South African communities. Citizens can trigger SOS alerts, report incidents, and view a live community crime map — while call centre operators and responders manage everything from two dedicated web dashboards. Built with **React Native (Expo)** for mobile and **React** for both dashboards, powered by **Firebase** on the backend.
 
---
 
## 💡 What It Does
 
SOS South Africa has three parts working together in real time:
 
**📱 Mobile App — for citizens**
Open the app, hit SOS, describe your emergency, and the system instantly locates the nearest emergency station to you. The responder is dispatched and you can track them live. If you're too shaken to call, the app automatically surfaces a call option 10 seconds after your request. Citizens can also access the Community Crime Map to view and report incidents — registration required to keep the community safe from anonymous actors.
 
**🖥️ Call Centre Dashboard — for operators**
A live overview of all active SOS alerts, incident locations on a map, and a full activity feed. Call centre operators can see every emergency as it comes in, track its status, and coordinate response in real time.
 
**🖥️ Responder Dashboard — for police & medics**
Responders log in, see incoming emergencies assigned to them, accept the call, and Google Maps guides them directly to the scene.
 
---
 
## 📸 Screenshots
 
### 📱 Mobile App — SOS Emergency Flow
 
#### 1. Welcome & Get Started
 
<img src="https://github.com/user-attachments/assets/f204c6f6-b638-4df5-ba0a-580dbdfb109c" width="300" alt="SOS Alert Welcome Screen" />
---
 
#### 2. Describe Your Emergency
> Select your emergency type and send the alert
 
<img src="https://github.com/user-attachments/assets/84f3d353-4704-455f-8554-0b4d6b9be552" width="300" alt="Describe Your Emergency" />
---
 
#### 3. Locating Nearest Emergency Station
> The app finds the closest available station to your GPS location
 
<img src="https://github.com/user-attachments/assets/1dee6a90-c03b-479c-9cf5-da1cc3ecf5e7" width="300" alt="Locating Nearest Emergency Station" />
---
 
#### 4. Station Located — Help Is On The Way
> Confirmation that a station has been found and a responder is dispatched
 
<img src="https://github.com/user-attachments/assets/ef7597ed-4c39-42e1-8073-a027b19b5683" width="300" alt="Emergency Station Located" />
---
 
#### 5. Live Route Tracking
> Track the responder live as they make their way to you
 
<img src="https://github.com/user-attachments/assets/66c74880-6090-4644-9c12-8550e81021f9" width="300" alt="Live Route Tracking" />
---
 
#### 6. Auto Call Option — Appears After 10 Seconds
> For citizens who are too shaken to act, the call option automatically appears 10 seconds after the SOS request
 
<img src="https://github.com/user-attachments/assets/28b1edd6-b694-459f-91fe-9b31b5818bb8" width="300" alt="Auto Call Option After 10 Seconds" />
---
 
### 📱 Mobile App — Community Crime Map
 
> Accessible from the **Alerts** button on the main page. Citizens can view reported incidents and report new ones. If **3 or more crimes** are reported in the same area, that area is automatically flagged as a **hotspot** with a red circle. Registration is required to report — keeping the community safe from anonymous actors.
 
---
 
#### Community Crime Map
 
<img src="https://github.com/user-attachments/assets/8f1923e9-5317-4fe1-9d4a-9a4005c8bd4c" width="300" alt="Community Crime Map" />
---
 
#### Report an Incident
 
<img src="https://github.com/user-attachments/assets/de608d73-e470-4686-a5ed-58284ec9c20f" width="300" alt="Report Incident Form" />
---
 
#### Crime Hotspot — 3+ Reports in One Area
> Areas with 3 or more crime reports are automatically marked with a red hotspot circle
 
<img src="https://github.com/user-attachments/assets/5e8a2b6c-57a7-446d-b837-b841bd4384dc" width="300" alt="Crime Hotspot Red Circle" />
---
 
#### 🔒 Access Restricted
> You must complete your profile before reporting crimes — this keeps the community safe from anonymous actors
 
<img src="https://github.com/user-attachments/assets/fac27063-6477-4b80-bba1-cda51793cb3a" width="300" alt="Access Restricted Screen" />
---
 
### 🖥️ Call Centre Dashboard
 
> Operators see every active SOS alert, track incidents on a live map, and coordinate emergency response in real time
 
<img src="https://github.com/user-attachments/assets/fe7a48aa-2f3d-49b5-ace2-51e70c7b897b" width="100%" alt="Call Centre Dashboard" />
---
 
### 🖥️ Responder Dashboard
 
> Police and medics log in, see emergencies assigned to them, accept the call, and are guided to the scene via Google Maps
 
<img src="https://github.com/user-attachments/assets/e16e10ef-8e5e-42d6-8ca2-c0c2df53b040" width="100%" alt="Responder Dashboard Overview" />
<img src="https://github.com/user-attachments/assets/3f57fd74-5828-48f2-a075-1f7954cc38e2" width="100%" alt="Responder Dashboard Incidents" />
<img src="https://github.com/user-attachments/assets/0871e868-1b4b-4aa0-822f-974f8f0e8579" width="100%" alt="Responder Dashboard Map View" />
<img src="https://github.com/user-attachments/assets/25b61e55-322b-46ad-b034-b77d18025354" width="100%" alt="Responder Dashboard Route Guidance" />
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
Call Centre Dashboard monitors all emergencies in real time
              ↓
Responder Dashboard guides police / medics to the scene
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

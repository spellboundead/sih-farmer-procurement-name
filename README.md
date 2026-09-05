# sih-farmer-procurement-name
# 🌾 KISAN RAKSHAK

### From Crop to Bank — Every Step Visible.

Kisan Rakshak is a farmer-centric digital transparency platform designed to help farmers track their crop procurement journey and payment status from crop submission to bank credit.

It acts as a **bridge between farmers and existing procurement systems**, making complex procurement and payment processes simple, transparent, and understandable.

---

## 🎯 Problem Statement

Farmers often face uncertainty after submitting their crops for procurement.

They may not know:

- 📦 Where their crop is in the procurement process
- 🔍 Whether quality verification is completed
- ⚖️ Whether their crop has been weighed
- ✅ Whether procurement has been accepted
- 💰 How much payment is expected
- 🏦 Whether the payment has reached their bank account
- ⏳ Why a payment is delayed
- 📢 Where to raise a grievance

This lack of visibility can lead to repeated visits to procurement centres and unnecessary uncertainty.

---

## 💡 Our Solution

**Kisan Rakshak** provides a simple farmer-facing platform that tracks the complete journey:

```text
Farmer
   ↓
Crop Submission
   ↓
Verification
   ↓
Quality Check
   ↓
Weighment
   ↓
Procurement Accepted
   ↓
MSP Amount Calculated
   ↓
Payment Authorization
   ↓
Bank Processing
   ↓
Amount Credited
````

The platform converts this complex process into a simple visual timeline that farmers can easily understand.

---

## 🚀 Key Features

### 👨‍🌾 Farmer Dashboard

* Farmer profile
* Crop details
* Quantity submitted
* Procurement status
* Expected MSP amount
* Payment status

### 📦 Crop Tracking

Farmers can track their crop through every major stage of procurement.

### 💰 MSP Tracking

The platform displays the applicable MSP and provides an estimated procurement value based on eligible quantity.

> MSP values shown in the prototype are demo/mock data. Actual MSP data would be obtained from authorized government sources during deployment.

### 🏦 Payment Tracking

Farmers can see whether their payment is:

* Pending
* Under processing
* Authorized
* Sent to bank
* Credited
* Failed

### 🤖 AI / Voice Assistant

A simple conversational assistant helps farmers:

* Check crop status
* Check payment status
* Understand delays
* Navigate the platform
* Raise grievances
* Interact using local languages

### 🌐 Multilingual Support

Designed for accessibility with support for:

* English
* Telugu
* Hindi

The system can be extended to additional Indian languages.

### 📱 QR-Based Tracking

A QR-based mechanism can be used to quickly access a farmer's procurement record or transaction status.

### 📢 Grievance Management

Farmers can raise issues related to:

* Procurement delays
* Payment delays
* Verification problems
* Quantity/quality issues
* Bank/payment failures

Each grievance can receive a tracking ID.

### 🔔 Notifications

Farmers can receive important updates regarding procurement and payment progress.

---

## 🔐 Security & Privacy

Kisan Rakshak follows a security-by-design approach.

The production architecture is designed to include:

* 🔑 Secure API key management
* 🛡️ Authentication and authorization
* 🔒 Encryption of sensitive information
* 🗄️ Database Row-Level Security (RLS)
* 👤 Role-based access control
* 🔐 Secure session management
* 🔑 Password hashing using Argon2id/bcrypt
* 🚦 Login rate limiting
* 🤖 Bot protection
* 🧹 Input validation and sanitization
* 🛡️ Protection against SQL injection
* 📁 Secure file-upload restrictions
* 📋 Minimal API responses
* 🧱 Security headers
* 📝 Audit logging
* 🎭 Masking of sensitive bank information

### Important

The current project is a prototype. Production-level authentication, database security, encryption, and government-system integration must be implemented on the backend.

---

## 🏗️ System Architecture

```text
              ┌──────────────────┐
              │      FARMER      │
              └────────┬─────────┘
                       ↓
              ┌──────────────────┐
              │ KISAN RAKSHAK UI │
              └────────┬─────────┘
                       ↓
              ┌──────────────────┐
              │     BACKEND      │
              │     / API        │
              └────────┬─────────┘
                       ↓
        ┌──────────────────────────────┐
        │ Government / Authorized Data │
        │ Procurement & Payment Systems│
        └──────────────┬───────────────┘
                       ↓
              ┌──────────────────┐
              │ KISAN RAKSHAK   │
              │ Transparency    │
              │     Layer        │
              └────────┬─────────┘
                       ↓
              ┌──────────────────┐
              │      FARMER      │
              └──────────────────┘
```

---

## 🛠️ Technology Stack

### Frontend

* HTML
* CSS
* JavaScript
* Responsive UI

### Proposed Production Frontend

* React
* TypeScript
* Tailwind CSS

### Backend

* FastAPI
* Python

### Database

* PostgreSQL

### AI / Voice

* Speech-to-Text
* Natural Language Processing
* Text-to-Speech
* Multilingual conversational interface

### Security

* Secure authentication
* HTTPS/TLS
* Database Row-Level Security
* Encryption
* Server-side validation
* Rate limiting

---

## 📊 Example Demo

### Farmer

**Ramesh Kumar**

* Location: Telangana
* Crop: Paddy
* Quantity: 54 Quintals
* Farmer ID: KR10245
* Transaction ID: KR-TG-2026-00078231

### Example Status

```text
✅ Crop Submitted
✅ Verification Completed
✅ Quality Check Completed
✅ Weighment Completed
✅ Procurement Accepted
✅ MSP Calculated
🟡 Payment Authorization Pending
⚪ Bank Credit
```

The farmer can immediately understand where the process is currently waiting.

---

## 🤖 AI Safety Principle

AI is used as an **accessibility and assistance layer**, not as the source of financial truth.

The AI should never invent:

* Payment amounts
* Transaction status
* Procurement status
* Bank information
* Government decisions

Verified procurement and payment information must come from structured backend data.

The AI simply explains that information to the farmer in an easy-to-understand way.

---

## 🌱 Impact

Kisan Rakshak aims to:

* Reduce uncertainty for farmers
* Reduce unnecessary visits to procurement centres
* Improve transparency in procurement
* Make payment status easier to understand
* Improve grievance tracking
* Support local-language access
* Help identify procurement/payment bottlenecks
* Improve trust between farmers and the procurement ecosystem

---

## ⚡ Why Kisan Rakshak?

Existing government systems already perform procurement and payment operations.

**Kisan Rakshak does not replace them.**

Instead, it creates a farmer-friendly transparency layer that makes the existing process:

**Visible → Trackable → Understandable → Accessible**

### Our core idea:

> **"We don't replace the procurement system. We make it visible to the farmer."**

---

## 🔮 Future Scope

* Integration with authorized government APIs
* Real-time procurement tracking
* Real-time payment status
* More Indian languages
* SMS and IVR support
* Offline/low-connectivity support
* CSC/procurement-centre assisted access
* Advanced grievance analytics
* Government bottleneck monitoring
* Mobile application
* Secure Aadhaar-based authentication where legally and operationally appropriate
* Integration with authorized bank/payment infrastructure

---

## ⚠️ Prototype Disclaimer

This project is a **prototype/demo implementation** developed to demonstrate the proposed concept and user experience.

The prototype uses simulated/demo procurement and payment data.

It does **not** directly procure crops, transfer money, or bypass existing government procurement systems.

A production deployment would require:

* Authorized government integration
* Approved APIs/data-sharing mechanisms
* Production backend infrastructure
* Proper authentication
* Database security
* Compliance with applicable data-protection requirements

---

## 🚀 How to Run

### Option 1 — Open Locally

1. Download/clone the repository.
2. Open the project folder.
3. Open `index.html` in a browser.

### Option 2 — VS Code

1. Open the project in VS Code.
2. Open `index.html`.
3. Use **Live Server** or open the HTML file directly in your browser.

---

## 📁 Project Structure

```text
KISAN-RAKSHAK/
│
├── index.html
├── README.md
└── assets/
    └── images/
```

For the current prototype, most functionality is contained within the single HTML file.

---

## 👥 Team

**Team Name:** Mission Possible

**Project:** Kisan Rakshak

**Hackathon:** Smart India Hackathon 2026

---

## ❤️ Vision

### A transparent procurement journey for every farmer.

**From Crop to Bank — Every Step Visible.**

🌾 **KISAN RAKSHAK**

```
```



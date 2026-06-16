# 🏥 Docly — Smart Clinic Management System

> A full-featured, single-file clinic reception & patient management system with role-based access, real-time dashboard, PDF prescriptions, and WhatsApp integration.

---

## 📖 About

Docly replaces manual diary-based patient record keeping in small clinics with a fast, modern digital solution. Built for receptionists and clinic admins — no technical knowledge required to use it.

It features three access levels: **Developer**, **Receptionist**, and a **Software Freeze** system — making it usable as a real deployable SaaS product.

---

## ✨ Features

### 🔐 Authentication & Access Control
- Role-based login — **Developer** and **Receptionist** accounts
- Secure credential management with password change support
- **Software Freeze** — Developer can lock out receptionist access remotely
- Frozen access screen with support contact button

### 📊 Dashboard
- Live stats — Total Visits, Pending, Completed, Revenue (₹)
- **Date range filter** — view records for any custom period
- Patient queue table with token numbers
- Mark patient as Done directly from dashboard
- One-click **Send Prescription** per patient

### 👤 Patient Registration
- Auto-generated unique Token ID (e.g. A-01, A-02...)
- Captures: Name, Age, Phone, Address, Doctor, Fees
- Payment method — **Cash** or **UPI** with Transaction ID
- Timestamped visit records

### 🔍 Patient Search & History
- Search by Name, Phone, or Token ID
- Full visit history timeline per patient
- Add new visit for returning patients via Quick Visit modal

### 💊 Prescription & WhatsApp
- Add medicines with dosage details
- Auto-generates professional **PDF prescription** (jsPDF)
- One-click **WhatsApp message** to patient's phone number
- PDF includes clinic name, doctor, patient details, medicine table

### 📤 Data Export
- Export all patient records to **Excel (.xlsx)**
- Full visit history included per patient

### 🔔 Developer Notifications
- Developer can send priority notifications (High / Medium / Low)
- Notification badge with unread count
- Mark all read functionality

### ⚙️ Settings
- Dark mode toggle
- Add / Remove doctors from the system
- Change username and password

---

## 🛠️ Tech Stack

| Technology | Usage |
|-----------|-------|
| HTML5, CSS3 | Structure & styling |
| Vanilla JavaScript | All logic & state management |
| Tailwind CSS (CDN) | Utility-first styling |
| Font Awesome | Icons |
| jsPDF + AutoTable | PDF prescription generation |
| SheetJS (XLSX) | Excel export |
| SweetAlert2 | Popup dialogs |
| localStorage | Client-side data persistence |
| WhatsApp API | Patient messaging via wa.me |

---

## 🏗️ System Architecture

```
Docly (Single File Application)
│
├── Auth Layer
│   ├── Developer Login  →  Full system access
│   └── Receptionist Login  →  Patient management only
│
├── Dashboard
│   ├── Stats (Visits, Revenue, Pending, Completed)
│   ├── Date Filter
│   └── Patient Queue Table
│
├── Patient Management
│   ├── New Registration (Token generation)
│   ├── Search & History
│   └── Quick Visit (returning patients)
│
├── Prescription Engine
│   ├── Medicine entry form
│   ├── PDF generation (jsPDF)
│   └── WhatsApp send link
│
└── Developer Dashboard
    ├── Manage credentials
    ├── Software freeze toggle
    └── Push notifications
```

---

## 🚀 How To Use

**Option 1 — Direct (No setup needed)**
1. Download `index.html`
2. Open in any browser
3. Login with default credentials:
   - Receptionist: `aks` / `aks`
   - Developer: `aksbytes` / `aksbytes`
4. Change credentials from Settings after first login

**Option 2 — Deploy**
- Upload `index.html` to any static hosting (Netlify, GitHub Pages, Vercel)
- No backend or database required — runs entirely in the browser

---

## 📸 Screenshots

> *(Add screenshots of Dashboard, Patient Registration, Prescription Modal here)*

---

## 💡 What I Built & Learned

- **Single File Architecture** — entire app (UI + logic + state) in one HTML file, no build tools needed
- **Role-Based Access Control** from scratch using vanilla JS
- **PDF generation** in the browser using jsPDF with AutoTable plugin
- **localStorage state management** — structured like a mini-database with patients, visits, settings, credentials
- **SaaS-style features** — software freeze, developer dashboard, push notifications
- **WhatsApp Business API** integration using `wa.me` deep links
- **Responsive design** — works on desktop and mobile with dynamic layout adjustments

---

## 👨‍💻 Author

**AaryanKumar Singh**
BSC IT — Mumbai University
[GitHub](https://github.com/aaryan-singh123) · [Email](mailto:aaksingh909@gmail.com)

---

> *"Built for a real clinic — designed to replace paper registers with a modern digital system."* 🏥

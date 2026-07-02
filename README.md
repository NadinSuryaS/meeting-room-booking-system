# 🏢 Meeting Room Booking System

<div align="center">

![ServiceNow](https://img.shields.io/badge/ServiceNow-App%20Engine%20Studio-009BDE?style=for-the-badge&logo=servicenow&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Now%20Platform-009BDE?style=for-the-badge&logo=servicenow&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**A fully automated Meeting Room Booking application built on ServiceNow App Engine Studio.**  
Digitalizes room reservations, eliminates double-booking, automates approvals, and provides real-time dashboards — all within the ServiceNow platform.

[📋 Features](#-features) • [🛠️ Tech Stack](#️-tech-stack) • [🔄 Workflow](#-workflow) • [📊 Modules](#-project-modules) • [🧪 Testing](#-testing) • [👤 Author](#-author)

---

</div>

## 📌 Project Overview

| Field | Details |
|---|---|
| **Project Name** | Meeting Room Booking System |
| **Platform** | ServiceNow App Engine Studio |
| **Application Type** | Custom Scoped Application |
| **Custom Table** | Meeting Room Booking |
| **Booking ID Format** | `MRB0001001`, `MRB0001002` … |
| **User Roles** | Employee (Requestor) · Administrator (Approver) |
| **Author** | Nadin Surya S |
| **Date** | June 2026 |

---

## 🚀 Features

| # | Feature | Description |
|---|---|---|
| 1 | 📝 **Booking Form** | Online form with Employee Name, ID, Email, Room, Date, Time & Purpose |
| 2 | ✅ **Client Script Validation** | Prevents submission when End Time ≤ Start Time |
| 3 | ⚙️ **Business Rule Automation** | Auto-assigns `Pending` status on every new booking |
| 4 | 🔄 **Flow Designer Workflow** | Automated workflow triggered on booking creation |
| 5 | 📧 **Email Notification** | Instant booking confirmation email sent to employee |
| 6 | 🔢 **Auto Number Generation** | Unique Booking ID generated automatically (prefix: `MRB`) |
| 7 | 👨‍💼 **Admin Approval** | Administrator reviews, approves and completes bookings |
| 8 | 📊 **Dashboard & Reports** | Status chart, room-wise chart, trend chart & booking list |
| 9 | 🔐 **Role-Based Access** | Separate access for Employee and Administrator roles |

---

## 🛠️ Tech Stack
┌─────────────────────────────────────────────────────────────┐
│                  ServiceNow Now Platform                     │
├──────────────────┬──────────────────┬───────────────────────┤
│   UI Layer       │   Logic Layer    │   Data Layer          │
│                  │                  │                        │
│  App Engine      │  Client Script   │  Custom Table         │
│  Studio UI       │  Business Rule   │  (Meeting Room        │
│  Booking Form    │  Flow Designer   │   Booking)            │
│                  │  Email Notif.    │  Auto Number          │
├──────────────────┴──────────────────┴───────────────────────┤
│   Reporting Layer: Dashboard · Reports · Charts             │
└─────────────────────────────────────────────────────────────┘

| Component | Technology |
|---|---|
| **Platform** | ServiceNow App Engine Studio |
| **UI** | Now Platform UI Builder (HTML, CSS, JS) |
| **Client Validation** | Client Script (JavaScript) |
| **Server Automation** | Business Rule (Server-side JavaScript) |
| **Workflow** | Flow Designer (ServiceNow Native) |
| **Database** | ServiceNow Custom Table |
| **Notifications** | ServiceNow Email Notification (SMTP) |
| **Reporting** | ServiceNow Reports & Dashboard |
| **Hosting** | ServiceNow Cloud (Multi-Instance) |

---

## 🔄 Workflow
Employee fills Booking Form
│
▼
Client Script validates End Time > Start Time
│
▼
Business Rule sets Status = Pending
│
▼
Flow Designer executes workflow
│
▼
Email Notification sent to Employee ──────────────────┐
│                                             │
▼                                             │
Booking stored in Meeting Room Booking Table     ✉️ Confirmation
│                                        sent instantly
▼
Administrator reviews Booking
│
▼
Administrator changes Status → Approved
│
▼
Meeting conducted in confirmed room
│
▼
Administrator marks Status → Completed
│
▼
Dashboard & Reports updated automatically ✅

---

## 📋 Booking Form Fields

| Field | Type | Description |
|---|---|---|
| `Number` | Auto Number | Unique Booking ID (MRB prefix) |
| `Employee Name` | String | Full name of the employee |
| `Employee ID` | String | Employee identifier |
| `Employee Email` | Email | For notification delivery |
| `Room Name` | Choice | Conference Room A / B, Training Room, Interview Room |
| `Booking Date` | Date | Date of the meeting |
| `Start Time` | Date/Time | Meeting start time |
| `End Time` | Date/Time | Meeting end time |
| `Purpose` | String | Reason for the meeting |
| `Status` | Choice | Pending / Approved / Completed |

---

## 📊 Project Modules
Phase 1 → Application Setup       ✅ App created, roles configured
Phase 2 → Database Design          ✅ Custom table, auto-numbering, fields
Phase 3 → Form Design              ✅ Booking form, mandatory fields, choices
Phase 4 → Business Logic           ✅ Client Script + Business Rule
Phase 5 → Workflow Automation      ✅ Flow Designer + Email Notification
Phase 6 → Reporting & Analytics    ✅ Dashboard + 4 Reports
Phase 7 → Testing & Validation     ✅ All 12 test cases passed

---

## 🧪 Testing

| Test Case | Module | Result |
|---|---|---|
| TC-01 | Submit valid booking form | ✅ Pass |
| TC-02 | Submit with missing mandatory field | ✅ Pass |
| TC-03 | End Time earlier than Start Time | ✅ Pass |
| TC-04 | End Time equal to Start Time | ✅ Pass |
| TC-05 | Business Rule — auto Pending status | ✅ Pass |
| TC-06 | Flow Designer execution on insert | ✅ Pass |
| TC-07 | Email Notification sent to employee | ✅ Pass |
| TC-08 | Auto Number generation (MRB format) | ✅ Pass |
| TC-09 | Admin approval — status to Approved | ✅ Pass |
| TC-10 | Admin marks booking Completed | ✅ Pass |
| TC-11 | Dashboard renders all charts | ✅ Pass |
| TC-12 | Booking Status Report generated | ✅ Pass |

**All 12 / 12 test cases passed ✅**

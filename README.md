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

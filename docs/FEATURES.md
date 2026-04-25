# StuSync Features

## Overview

StuSync is a comprehensive, offline-first school management system built specifically for Nepal's educational institutions. It handles every aspect of school administration — from admissions to finance, exams to transport — in a single, secure application.

---

## Core Modules

### 🎓 Registry (Student & Staff)

- **Student Profiles** — Full admissions data, photos, guardian contacts, emergency info, document storage
- **Staff Records** — Qualifications, contracts, attendance history, leave tracking
- **Admissions** — Digital admission forms, enrollment tracking
- **Transfers** — Student transfer requests and processing
- **Live Analytics** — Real-time enrollment statistics by grade, gender, section

### 📚 Academics (Exams & Marks)

- **Subject Management** — Subjects per grade/section, teacher assignments
- **Grading Scales** — Customizable GPA ranges, symbols, credit hours
- **Marks Entry** — Bulk import via CSV, per-student entry, class-wise entry
- **Report Cards** — Auto-generated marksheets with GPA calculation
- **Examinations** — Exam schedules, seating plans, admit cards
- **Certificates** — 9 professional templates (TC, character, bonafide, etc.)

### 💰 Finance

- **Fee Structure** — Class-wise fee setup, multiple heads
- **Invoicing** — Auto-generated fee bills, receipts
- **Payments** — Cash, bank, mobile payment tracking
- **Scholarships** — Automatic discounts, waiver management
- **Due Reports** — Automated due alerts
- **Expenses** — Expenditure tracking, category-wise reports
- **Wallet System** — Staff advances, salary deductions

### 🚌 Transport

- **Routes & Stops** — Define routes, assign stops, pickup points
- **Fleet Management** — Bus assignment, capacity tracking
- **GPS Monitoring** — Live map visualization (offline cached)
- **Student Assignment** — Per-student bus/stop assignment

### 📷 CCTV & Dashboard

- **Live Camera Feeds** — DVR/IP camera integration
- **Secondary Dashboard** — Multi-monitor support
- **Real-time Stats** — Live student count, today's attendance, collections

### 👨‍💼 Staff Management

- **Attendance** — Daily mark-in/mark-out, class-wise trends
- **Leave Management** — Leave requests, approval workflow
- **Payroll** — PL/LWP auto-calculation from attendance
- **Performance** — Staff ranking, evaluation tracking

### ☁️ Cloud Sync (Supabase)

- **Offline-First** — Works without internet
- **Smart Sync** — Only syncs changed data
- **Conflict Resolution** — Preserves data integrity
- **Multi-Device** — Sync across devices

### 🔒 Security & Licensing

- **Hardware-Linked License** — Machine-specific activation
- **Device Registry** — Track authorized devices
- **SQLCipher Encryption** — AES-256 local DB encryption
- **Role-Based Access** — Principal, Admin, Staff permissions
- **90-Day Audit Trail** — Every action logged
- **Server-Side Validation** — Supabase RLS policies

---

## Additional Features

### Parent Portal (Web)
- View child's attendance, marks, fee status
- Online fee payment integration
- Real-time notifications

### Mobile App (Coming Soon)
- Android & iOS for parents/students
- Attendance, marks, notices access

### GPS Live Tracking (In Development)
- Real-time bus location
- Parent alerts

### Advanced Analytics (Planned)
- AI-powered trend forecasting
- Enrollment, attendance, performance predictions

---

## Technical Specifications

| Property | Value |
|----------|-------|
| Platform | Windows Desktop (x64) |
| Framework | Flutter |
| Database | SQLite + SQLCipher |
| Cloud | Supabase |
| Encryption | AES-256 |
| License | Hardware-bound |

---

## Documentation

- [Installation Guide](./INSTALL.md)
- [Pricing Plans](./PRICING.md)
- [Security Policy](../SECURITY.md)

---

*© 2024–2026 Trehive*
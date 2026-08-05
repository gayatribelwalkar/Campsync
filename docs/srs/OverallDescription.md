# Overall Description
---

# Product Perspective
CampSync is a web-based Progressive Web Application (PWA) that supports offline healthcare operations.
The system consists of:
- Mobile application for field volunteers
- Web dashboard for NGO administrators
- Backend API
- PostgreSQL database
- IndexedDB offline database
- WhatsApp notification service

---
# Product Functions
CampSync provides the following functions:
- Patient Registration
- Medical Examination
- Equipment Management
- Referral Management
- Offline Data Entry
- Automatic Synchronization
- Dashboard Analytics
- Patient Feedback
- Report Generation

---
# User Classes
### Field Volunteer
Registers patients, records medical data, and works offline.
### NGO Administrator
Monitors healthcare camps, manages inventory, and generates reports.
### Patient
Receives medical services, referrals, and WhatsApp follow-up messages.
---

# Operating Environment
- Windows
- Android
- Chrome Browser
- Edge Browser
Backend
- Node.js
- PostgreSQL
- Redis

---
# Design Constraints
- Must support offline operation.
- Must synchronize automatically.
- Must support low-bandwidth environments.
- Must protect patient data.
- Must be responsive.

---
# Assumptions
- Volunteers possess Android smartphones.
- Internet is available periodically.
- NGO maintains a central server.
- Patients provide valid contact information.
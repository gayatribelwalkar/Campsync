# Functional Requirements
# CampSync: A Resilient, Low-Bandwidth Consolidated NGO Healthcare & Inventory System
---
## Introduction
Functional requirements describe the features and services that CampSync must provide to its users. These requirements define the expected behavior of the system.

---
# FR-01 User Authentication
The system shall allow NGO administrators and field volunteers to securely log in using their registered credentials.

---
# FR-02 Role-Based Access
The system shall provide different permissions for:
- NGO Administrator
- Field Volunteer
Each user shall only access features according to their assigned role.

---
# FR-03 Patient Registration
The system shall allow volunteers to register new patients by entering:
- Full Name
- Age
- Gender
- Mobile Number
- Address
- Emergency Contact
- Aadhaar/Unique Patient ID (if available)
---

# FR-04 Patient Search
The system shall allow volunteers to search patients using:
- Name
- Phone Number
- Patient ID
The search shall work even in offline mode using IndexedDB.

---
# FR-05 Medical Examination
The system shall record:
- Blood Pressure
- Blood Sugar
- SpO₂
- Weight
- Temperature
- Doctor Notes
- Diagnosis

---
# FR-06 Hospital Referral
The system shall allow doctors or volunteers to refer patients to partner hospitals.
The referral shall include:
- Hospital Name
- Referral Date
- Reason
- Priority Level

---
# FR-07 Medical Equipment Request
The system shall allow volunteers to request equipment such as:
- Wheelchair
- Walker
- Crutches
- Oxygen Concentrator
- Hospital Bed

---
# FR-08 Inventory Management
The administrator shall:
- Add equipment
- Update equipment
- Assign equipment
- Return equipment
- Mark maintenance status

---
# FR-09 Equipment Tracking
The system shall maintain the current status of every equipment item.
Possible statuses include:
- Available
- Assigned
- Maintenance
- Lost

---
# FR-10 Offline Data Entry
The system shall continue working without internet connectivity.
All entered records shall be stored locally.

---
# FR-11 Automatic Synchronization
When internet connectivity is restored, the system shall automatically synchronize offline records with the central server.

---
# FR-12 Synchronization Status
The application shall display synchronization status, including:
- Records Pending
- Sync in Progress
- Sync Successful
- Sync Failed

---
# FR-13 Dashboard
The administrator dashboard shall display:
- Active Camps
- Total Patients
- Equipment Status
- Pending Referrals
- High-Risk Patients

---
# FR-14 WhatsApp Notification
The system shall automatically send WhatsApp messages for:
- Referral reminders
- Equipment follow-up
- Feedback requests

---
# FR-15 Reports
The system shall generate reports including:
- Camp Summary
- Patient Statistics
- Equipment Reports
- Referral Reports

---
# FR-16 Audit Log
The system shall maintain logs of important user activities.
---

# FR-17 Data Backup
The backend shall periodically back up patient and inventory data.

---
# FR-18 Error Handling
The system shall display meaningful error messages and allow users to retry failed operations.

---
# FR-19 Notifications
The administrator shall receive notifications regarding:
- Pending Synchronizations
- Equipment Shortages
- High-Risk Patients

---
# FR-20 Logout
The system shall allow authenticated users to securely log out.
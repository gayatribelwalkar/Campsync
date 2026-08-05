# Use Cases
# CampSync: A Resilient, Low-Bandwidth Consolidated NGO Healthcare & Inventory System

---
# Introduction
A use case describes how a user interacts with the CampSync system to accomplish a specific task. The primary actors are:
- Field Volunteer
- NGO Administrator
- Patient

---
# UC-01 User Login
### Primary Actor
Field Volunteer / NGO Administrator
### Description
The user logs into the CampSync system using valid credentials.
### Preconditions
- User account exists.
- User is registered.
### Main Flow
1. User enters username/email.
2. User enters password.
3. System verifies credentials.
4. User is redirected to the dashboard.
### Postconditions
- User is successfully authenticated.
- Dashboard is displayed.

---
# UC-02 Register Patient
### Primary Actor
Field Volunteer
### Description
Register a new patient during a healthcare camp.
### Preconditions
- Volunteer is logged in.
### Main Flow
1. Open Registration Screen.
2. Enter patient details.
3. Enter contact information.
4. Save patient record.

### Postconditions
- Patient record is stored locally or on the server.
---

# UC-03 Search Patient
### Primary Actor
Field Volunteer
### Description
Search an existing patient using Name, Mobile Number, or Patient ID.
### Preconditions
- Volunteer is logged in.
### Main Flow
1. Open Search Screen.
2. Enter search keyword.
3. System displays matching patients.
4. Volunteer selects a patient.
### Postconditions
- Patient record is opened.
---

# UC-04 Record Medical Examination
### Primary Actor
Field Volunteer
### Description
Record the patient's medical examination.
### Main Flow
1. Open patient profile.
2. Enter vital signs.
3. Record doctor's notes.
4. Save examination.

### Postconditions
- Medical record is saved.
---

# UC-05 Hospital Referral
### Primary Actor
Field Volunteer
### Description
Refer a patient to a hospital for advanced treatment.
### Main Flow
1. Select patient.
2. Choose referral hospital.
3. Enter referral reason.
4. Save referral.

### Postconditions
- Referral record is created.
---

# UC-06 Equipment Assignment
### Primary Actor
NGO Administrator
### Description
Assign medical equipment to a patient.
### Main Flow
1. Open inventory.
2. Select equipment.
3. Select patient.
4. Confirm assignment.
### Postconditions
- Equipment status changes to Assigned.

---
# UC-07 Inventory Management
### Primary Actor
NGO Administrator
### Description
Manage donated medical equipment.
### Main Flow
1. Add equipment.
2. Update equipment.
3. Remove equipment.
4. View inventory status.

### Postconditions
- Inventory database is updated.
---

# UC-08 Offline Data Entry
### Primary Actor
Field Volunteer
### Description
Continue using CampSync without internet.
### Main Flow
1. Internet becomes unavailable.
2. Volunteer continues working.
3. Records are stored in IndexedDB.
### Postconditions
- Offline records are safely stored.

---
# UC-09 Data Synchronization
### Primary Actor
System
### Description
Automatically synchronize offline records.
### Preconditions
- Internet connection is restored.
### Main Flow
1. Service Worker detects connectivity.
2. Pending records are uploaded.
3. Backend validates data.
4. PostgreSQL is updated.
5. Sync status changes to Successful.
### Postconditions
- Offline records are synchronized.

---
# UC-10 Dashboard Monitoring
### Primary Actor
NGO Administrator
### Description
Monitor healthcare camps using the dashboard.
### Main Flow
1. Open Dashboard.
2. View patient statistics.
3. View inventory.
4. View high-risk patients.
5. View reports.
### Postconditions
- Administrator receives real-time insights.

---
# UC-11 WhatsApp Follow-Up
### Primary Actor
System
### Description
Automatically send follow-up messages to patients.
### Main Flow
1. Equipment assigned.
2. Follow-up schedule created.
3. WhatsApp message sent.
4. Patient responds.
5. Dashboard updates.
### Postconditions
- Feedback is recorded.

---
# UC-12 Generate Reports
### Primary Actor
NGO Administrator
### Description
Generate healthcare camp reports.
### Main Flow
1. Select report type.
2. Select date range.
3. Generate report.
4. Download report.
### Postconditions
- Report is generated successfully.

---
# UC-13 Logout
### Primary Actor
All Users
### Description
Log out of the system securely.
### Main Flow
1. Click Logout.
2. Session ends.
3. Login screen appears.
### Postconditions
- User session is terminated.

---
# Summary
These use cases define the major interactions between users and the CampSync system. They provide the foundation for the Use Case Diagram, Activity Diagram, Sequence Diagram, frontend interface design, backend APIs, and testing scenarios.
# Use Case Specification

## Project Title
**CampSync: A Resilient, Low-Bandwidth Consolidated NGO Healthcare & Inventory Management System**
---
# 1. Introduction
The Use Case Specification defines the interactions between different users (actors) and the CampSync system. It describes the functionalities provided by the system and helps developers understand how different stakeholders interact with the application. This document serves as the foundation for designing the Use Case Diagram and implementing the system.

---
# 2. Actors
## 2.1 Field Volunteer
Field Volunteers are responsible for conducting healthcare camps and collecting patient information in offline mode.
**Responsibilities**
- Login to the system
- Register patients
- Search patient records
- Update patient information
- Record patient vital signs
- Manage camp activities
- Update inventory usage
- Synchronize offline data

---
## 2.2 NGO Administrator
NGO Administrators manage healthcare camps and monitor overall system activities.
**Responsibilities**
- Login
- Manage healthcare camps
- Manage volunteers
- Allocate medical equipment
- View dashboard
- Generate reports
- Monitor referrals
- Manage inventory

---
## 2.3 Doctor
Doctors provide healthcare services during camps.
**Responsibilities**
- View patient records
- Record diagnosis
- Prescribe medicines
- Recommend hospital referral
- Update treatment details

---
## 2.4 Patient
Patients receive healthcare services.
**Responsibilities**
- Register for healthcare camp
- Receive treatment
- Receive hospital referral
- Receive WhatsApp follow-up reminders
- Submit feedback

---
## 2.5 Hospital
Partner hospitals receive referred patients.
**Responsibilities**
- Receive referral information
- Update referral status
- Share treatment outcome

---
# 3. Use Cases
## Authentication
- UC-01 Login
- UC-02 Logout

---
## Patient Management
- UC-03 Register Patient
- UC-04 Search Patient
- UC-05 Update Patient Details
- UC-06 View Patient History

---
## Camp Management
- UC-07 Create Healthcare Camp
- UC-08 Manage Camp
- UC-09 Assign Volunteers

---
## Inventory Management
- UC-10 Add Medical Equipment
- UC-11 Allocate Equipment
- UC-12 Update Inventory
- UC-13 View Inventory

---
## Hospital Referral
- UC-14 Create Referral
- UC-15 Track Referral
- UC-16 Update Referral Status

---
## Feedback Management
- UC-17 Send WhatsApp Reminder
- UC-18 Collect Patient Feedback

---
## Reports
- UC-19 Generate Reports
- UC-20 View Dashboard

---
## Synchronization
- UC-21 Synchronize Offline Data

---
# 4. Actor – Use Case Mapping
| Use Case | Volunteer | Admin | Doctor | Patient | Hospital |
|-----------|:---------:|:-----:|:-------:|:-------:|:--------:|
| Login | ✓ | ✓ | ✓ | | |
| Register Patient | ✓ | | | ✓ | |
| Search Patient | ✓ | ✓ | ✓ | | |
| Update Patient | ✓ | | ✓ | | |
| View Patient History | | | ✓ | | |
| Create Camp | | ✓ | | | |
| Manage Camp | ✓ | ✓ | | | |
| Add Equipment | | ✓ | | | |
| Allocate Equipment | ✓ | ✓ | | | |
| Update Inventory | ✓ | ✓ | | | |
| Create Referral | | | ✓ | | |
| Track Referral | ✓ | ✓ | ✓ | | ✓ |
| Send WhatsApp Reminder | | ✓ | | ✓ | |
| Generate Reports | | ✓ | | | |
| View Dashboard | | ✓ | | | |
| Synchronize Offline Data | ✓ | | | | |

---
# 5. Include Relationships
### Register Patient includes
- Validate Patient Details
- Generate Patient ID
- Save Patient Record

### Create Referral includes
- Select Hospital
- Update Patient Record
- Send Referral Details

### Allocate Equipment includes
- Check Inventory
- Update Stock
- Save Allocation Details

### Generate Reports includes
- Retrieve Records
- Generate Charts
- Export Report

---
# 6. Extend Relationships
### Register Patient extends
- Create Hospital Referral (if required)

### Register Patient extends
- Send WhatsApp Reminder (if patient provides mobile number)

### Allocate Equipment extends
- Low Stock Alert

### Synchronize Offline Data extends
- Conflict Resolution

---
# 7. System Boundary
The CampSync system consists of the following modules:
- Authentication
- Patient Management
- Camp Management
- Inventory Management
- Hospital Referral
- Feedback Management
- Dashboard & Analytics
- Offline Synchronization

External entities interacting with the system include:
- Field Volunteer
- NGO Administrator
- Doctor
- Patient
- Hospital
- WhatsApp Service

---
# 8. Assumptions
- Volunteers use smartphones or tablets.
- NGO administrators use desktops or laptops.
- Internet connectivity may not be available during healthcare camps.
- Offline data is synchronized automatically when connectivity is restored.
- WhatsApp is available for patient communication.

---
# 9. Constraints
- Limited internet connectivity.
- Low-bandwidth environments.
- Secure handling of patient information.
- Offline-first architecture.
- Limited storage on mobile devices.

---
# 10. Benefits of Use Case Modeling
- Provides a clear understanding of system functionality.
- Improves communication among stakeholders.
- Simplifies software design.
- Helps during system testing.
- Reduces ambiguity in software requirements.
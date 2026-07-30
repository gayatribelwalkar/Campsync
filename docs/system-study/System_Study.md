# System Study

# CampSync: A Resilient, Low-Bandwidth Consolidated NGO Healthcare & Inventory System

---

# 1. Introduction

Healthcare camps organized by Non-Governmental Organizations (NGOs) play an essential role in providing affordable or free medical services to underserved communities, particularly in rural and urban slum areas. During these camps, volunteers register patients, doctors record medical observations, equipment is distributed, and patients are referred to hospitals when necessary.

However, many NGOs continue to depend on paper records, spreadsheets, multiple WhatsApp groups, and separate software applications. These disconnected methods make healthcare management slow, error-prone, and difficult to monitor.

CampSync is proposed as an integrated offline-first healthcare management system that allows NGOs to perform all camp-related activities through a single digital platform.

---

# 2. Why This Topic?

The motivation for developing CampSync originates from real-world observations during community service at Ravindra Joshi Medical Foundation (RJMF).

During the community service, several operational challenges were observed:

- Patient information was initially recorded manually on paper.
- Google Sheets was introduced to improve digital record keeping.
- WhatsApp groups were created to collect patient feedback regarding donated medical equipment.
- Volunteers manually managed patient registrations and referrals during healthcare camps.
- Medical equipment allocation and follow-up activities were maintained separately.

These observations highlighted the absence of an integrated healthcare management system specifically designed for NGO-operated medical camps.

CampSync aims to eliminate fragmented workflows by combining patient registration, medical record management, equipment inventory, hospital referrals, and patient follow-up within a unified platform.

---

# 3. Topic Background

Healthcare NGOs frequently organize outreach camps in remote villages and urban slums where internet connectivity is unreliable or completely unavailable.

Traditional hospital management systems assume continuous internet connectivity and permanent healthcare facilities. These assumptions do not hold true for temporary healthcare camps.

Modern web technologies such as Progressive Web Applications (PWAs), IndexedDB, and Service Workers provide an opportunity to build applications capable of functioning offline while synchronizing data automatically once connectivity is restored.

CampSync utilizes these technologies to enable uninterrupted healthcare operations regardless of network availability.

---

# 4. Problem Context

Current NGO healthcare operations experience several challenges:

- Paper-based patient registration is time-consuming.
- Patient records are scattered across notebooks, spreadsheets, and messaging applications.
- Medical equipment allocation lacks centralized tracking.
- Volunteers struggle to update records in areas without internet access.
- Patient follow-up depends on manual phone calls or WhatsApp messages.
- Administrators have limited visibility into ongoing healthcare camps.
- Decision-making is delayed due to fragmented information.

These issues reduce operational efficiency and increase the possibility of data duplication, equipment loss, and missed patient follow-ups.

CampSync addresses these problems through an integrated offline-first digital healthcare ecosystem.

---

# 5. Target Users

CampSync is designed for three primary stakeholders involved in NGO healthcare operations.

## 5.1 Field Volunteers

Field volunteers are responsible for registering patients, recording medical information, updating treatment details, and managing healthcare camp operations. Since healthcare camps are often conducted in areas with poor or no internet connectivity, volunteers require an application that functions completely offline while remaining simple and fast to use.

### Requirements

- Smartphone or tablet support
- Large touch-friendly interface
- Offline patient registration
- Fast local patient search
- Automatic synchronization after internet recovery

---

## 5.2 NGO Administrators

NGO administrators monitor multiple healthcare camps, manage medical equipment inventory, assign donated equipment to patients, monitor referrals, and generate reports for decision making.

### Requirements

- Desktop dashboard
- Real-time analytics
- Inventory management
- Referral monitoring
- Volunteer activity tracking

---

## 5.3 Patients

Patients are beneficiaries of healthcare camps organized by NGOs.

Patients receive:

- Medical consultation
- Hospital referrals
- Donated medical equipment
- Follow-up notifications
- Feedback surveys through WhatsApp

---

# 6. Objectives of the System

The primary objective of CampSync is to develop an integrated healthcare management system capable of operating efficiently in low-bandwidth and offline environments.

Specific objectives include:

- Digitize patient registration during healthcare camps.
- Maintain centralized electronic patient records.
- Manage donated medical equipment inventory.
- Track hospital referrals.
- Provide offline-first functionality.
- Synchronize data automatically.
- Improve communication between volunteers and administrators.
- Automate patient follow-up using WhatsApp.
- Generate analytical reports for NGOs.

---

# 7. Tangible Benefits

The implementation of CampSync provides measurable benefits.

- Reduced patient registration time.
- Reduced paperwork.
- Faster healthcare camp operations.
- Improved inventory accuracy.
- Better equipment utilization.
- Faster report generation.
- Reduced data duplication.
- Reduced administrative workload.

---

# 8. Intangible Benefits

CampSync also provides qualitative benefits.

- Improved patient satisfaction.
- Better volunteer experience.
- Increased organizational transparency.
- Improved decision making.
- Higher trust among donors.
- Better coordination between NGO teams.
- Enhanced digital transformation.

---

# 9. Core Functionalities

The core functionalities of CampSync include:

1. Offline patient registration
2. Patient record management
3. Medical examination recording
4. Medical equipment inventory
5. Equipment allocation
6. Hospital referral management
7. Automatic synchronization
8. NGO admin dashboard
9. Patient follow-up
10. Report generation

---

# 10. Enhanced Features

Additional features include:

- Local fuzzy patient search
- IndexedDB offline storage
- Background synchronization
- WhatsApp Cloud API integration
- High-risk patient identification

---

# 11. Special Features

The unique features of CampSync are:

- 100% Offline-First Progressive Web Application
- Unified NGO healthcare ecosystem
- Integrated medical equipment lifecycle management
- Automated WhatsApp follow-up
- Real-time inventory analytics
- Low-bandwidth optimized architecture

---

# 12. Feasibility Study

## 12.1 Technical Feasibility

CampSync is technically feasible because it utilizes widely adopted open-source technologies.

### Frontend

- HTML5
- CSS3
- JavaScript
- React
- Progressive Web App (PWA)

### Backend

- Node.js
- Express.js

### Database

- PostgreSQL
- IndexedDB

### Additional Technologies

- Redis
- Service Workers
- WhatsApp Cloud API

These technologies are mature, scalable, well documented, and supported by large developer communities.

---

## 12.2 Operational Feasibility

CampSync is operationally feasible because volunteers require minimal technical knowledge.

The application uses:

- Large buttons
- High-contrast interface
- Dropdown selections
- Touch-friendly screens

making it suitable for field healthcare operations.

---

## 12.3 Economic Feasibility

CampSync minimizes development and operational costs by using open-source technologies.

No expensive software licenses are required.

The use of PWAs also eliminates the need for separate Android and iOS application development.

---

## 12.4 Schedule Feasibility

The project can be completed within one academic semester following the Software Engineering life cycle.

Major phases include:

- Research
- Requirement Analysis
- System Design
- Development
- Testing
- Documentation
- Final Deployment

---

# 13. Methodology

The CampSync project follows the Agile Software Development Methodology.

Reasons for selecting Agile include:

- Continuous development
- Incremental implementation
- Easy requirement changes
- Frequent testing
- Better stakeholder feedback
- Faster issue resolution

Each sprint focuses on completing a specific module while maintaining continuous documentation and GitHub version control.

---

# 14. Conclusion

The System Study demonstrates that CampSync is technically, operationally, economically, and practically feasible.

The project addresses real-world healthcare challenges observed during NGO healthcare camps by integrating patient management, inventory tracking, hospital referrals, and automated follow-up into a unified offline-first platform.

The findings from this study provide a strong foundation for the subsequent phases of requirement analysis, system design, implementation, testing, and deployment.
# Software Requirements Specification (SRS)
# Introduction

---
# 1. Purpose
The purpose of this Software Requirements Specification (SRS) is to define the functional and non-functional requirements of CampSync: A Resilient, Low-Bandwidth Consolidated NGO Healthcare & Inventory System.
This document serves as a reference for the design, development, testing, deployment, and maintenance of the system. It also ensures that all stakeholders have a common understanding of the project's objectives and expected functionality.

---
# 2. Scope
CampSync is an offline-first healthcare management system designed for NGOs conducting medical camps in rural and urban low-connectivity areas.
The system enables:
- Offline patient registration
- Medical record management
- Medical equipment inventory tracking
- Hospital referrals
- Automatic synchronization
- NGO administration dashboard
- WhatsApp-based patient follow-up
The application aims to replace paper records, spreadsheets, and fragmented communication with a unified digital platform.

---
# 3. Intended Audience
This document is intended for:
- Project Guide
- Software Developers
- Test Engineers
- NGO Administrators
- Field Volunteers
- Future Developers
- Project Evaluators

---
# 4. Definitions
| Term | Meaning |
|------|---------|
| NGO | Non-Governmental Organization |
| PWA | Progressive Web Application |
| IndexedDB | Browser-based offline database |
| Service Worker | Background browser process enabling offline functionality |
| REST API | Communication interface between frontend and backend |
| JWT | JSON Web Token |
| Sync | Transfer of offline data to cloud database |

---
# 5. References
This SRS is prepared using:
- Research papers collected during the literature review
- Software Engineering principles
- IEEE SRS recommendations
- Community observations from NGO healthcare camps
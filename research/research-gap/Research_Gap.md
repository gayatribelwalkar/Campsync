# Research Gap

## Introduction

A detailed review of twenty-two research papers related to healthcare information systems, Progressive Web Applications (PWAs), offline-first technologies, inventory management, NGO healthcare, mobile health (mHealth), and patient referral systems was conducted.

The review revealed that although several effective solutions exist, most of them focus on solving a single aspect of healthcare management rather than providing a complete end-to-end solution.

---

## Identified Research Gap

The existing literature can be broadly classified into two major categories.

### 1. Technical-Focused Systems
Several studies primarily concentrate on technical aspects such as:

- Offline synchronization
- Progressive Web Applications
- Service Workers
- IndexedDB
- Data security
- Electronic Health Records
- Mobile health applications

These systems demonstrate excellent technical performance but provide limited support for NGO healthcare operations and field camp management.

---

### 2. Management-Focused Systems

Another group of studies focuses on healthcare administration, including:

- Health camp organization
- Rural healthcare delivery
- NGO healthcare programs
- Pharmacy inventory
- Government collaboration

These studies explain organizational workflows but lack integrated software solutions capable of operating in low-bandwidth environments.

---

## Missing Features in Existing Systems

The literature review indicates that current systems generally lack one or more of the following capabilities:

- Offline patient registration
- Integrated patient medical records
- Donated medical equipment tracking
- Inventory allocation and maintenance
- Hospital referral management
- Automatic synchronization after network recovery
- WhatsApp-based patient follow-up
- Unified dashboard for NGO administrators
- Analytics for healthcare camps

No single system combines all these functionalities into one platform.

---

## How CampSync Addresses the Gap

CampSync proposes a unified offline-first healthcare ecosystem specifically designed for NGO-operated medical camps.

The proposed system integrates:

- Offline patient registration using IndexedDB
- Progressive Web Application (PWA) architecture
- Automatic synchronization using Service Workers
- Medical equipment inventory management
- Hospital referral tracking
- NGO administrative dashboard
- Patient feedback collection through WhatsApp Cloud API
- Real-time analytics for camp operations

Unlike existing research, CampSync combines healthcare delivery, inventory management, patient follow-up, and NGO administration within a single integrated platform.

---

## Conclusion

The identified research gap demonstrates the need for an integrated offline-first healthcare management system capable of supporting NGO medical camps operating in areas with limited or no internet connectivity.

CampSync is proposed to bridge this gap by providing a secure, scalable, and user-friendly platform that connects field volunteers, NGO administrators, and patients through a unified workflow.
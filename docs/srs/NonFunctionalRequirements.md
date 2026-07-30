# Non-Functional Requirements

# CampSync: A Resilient, Low-Bandwidth Consolidated NGO Healthcare & Inventory System

---

# Introduction

Non-functional requirements describe the quality attributes and operational characteristics of CampSync. These requirements define how well the system should perform rather than what functions it performs.

---

# NFR-01 Performance

The system shall:

- Load the dashboard within 3 seconds under normal network conditions.
- Display patient search results within 2 seconds.
- Save offline records within 1 second.
- Synchronize records efficiently after internet connectivity is restored.

---

# NFR-02 Reliability

The system shall:

- Continue functioning even when internet connectivity is unavailable.
- Prevent data loss during synchronization.
- Recover gracefully from synchronization failures.
- Maintain data consistency between offline and online databases.

---

# NFR-03 Availability

The system shall:

- Be available whenever healthcare camps are conducted.
- Allow uninterrupted offline usage.
- Automatically reconnect when the network becomes available.

---

# NFR-04 Scalability

The system shall support:

- Multiple NGOs
- Multiple healthcare camps
- Thousands of patient records
- Large equipment inventories
- Future expansion without major architectural changes

---

# NFR-05 Security

The system shall:

- Authenticate users before granting access.
- Encrypt communication using HTTPS.
- Store passwords securely using hashing techniques.
- Protect patient information from unauthorized access.
- Implement role-based access control.

---

# NFR-06 Usability

The application shall:

- Have a simple and intuitive interface.
- Use large touch-friendly buttons.
- Minimize typing by using dropdown menus and checkboxes.
- Be easy to use for volunteers with limited technical knowledge.
- Display clear status indicators for offline and online modes.

---

# NFR-07 Maintainability

The system shall:

- Use modular architecture.
- Follow coding standards.
- Maintain proper documentation.
- Support future feature additions with minimal changes.

---

# NFR-08 Portability

The application shall:

- Run on modern web browsers.
- Support Android devices through Progressive Web App installation.
- Operate across different operating systems without modification.

---

# NFR-09 Compatibility

CampSync shall be compatible with:

- Google Chrome
- Microsoft Edge
- Android smartphones
- Desktop computers
- PostgreSQL
- Node.js
- Redis

---

# NFR-10 Offline Capability

The system shall:

- Operate completely without internet.
- Store all offline records in IndexedDB.
- Synchronize automatically once internet connectivity is restored.

---

# NFR-11 Data Integrity

The system shall:

- Prevent duplicate patient records.
- Validate mandatory fields before saving.
- Preserve data consistency during synchronization.
- Maintain accurate inventory records.

---

# NFR-12 Backup and Recovery

The system shall:

- Perform regular database backups.
- Support data recovery in case of system failure.
- Maintain synchronization logs for troubleshooting.

---

# NFR-13 Accessibility

The system shall:

- Provide a high-contrast interface suitable for outdoor healthcare camps.
- Support readable fonts.
- Use icons and color indicators for quick understanding.

---

# NFR-14 Extensibility

The architecture shall support future integration with:

- AI-based disease prediction
- Government healthcare systems
- GIS mapping
- SMS and Email notifications
- Additional NGO branches

---

# NFR-15 Compliance

The system shall:

- Handle patient information responsibly.
- Follow standard software engineering practices.
- Maintain proper project documentation and version control using GitHub.

---

# Conclusion

These non-functional requirements ensure that CampSync is reliable, secure, scalable, maintainable, and suitable for deployment in offline healthcare environments. Together with the functional requirements, they provide a complete specification for the system's quality and operational expectations.
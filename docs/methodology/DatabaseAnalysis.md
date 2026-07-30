# Database Analysis

# CampSync: A Resilient, Low-Bandwidth Consolidated NGO Healthcare & Inventory System

---

# 1. Introduction

A database is the backbone of any information system. It is responsible for storing, organizing, retrieving, and managing data efficiently. Since CampSync operates in offline-first healthcare environments, the database design must support both local offline storage and centralized cloud storage while ensuring data consistency, security, and scalability.

CampSync adopts a hybrid database architecture consisting of PostgreSQL as the central database and IndexedDB as the offline local database.

---

# 2. Database Requirements

The database must support the following functionalities:

- Patient registration
- Medical record storage
- Camp management
- Volunteer information
- Medical equipment inventory
- Hospital referrals
- WhatsApp follow-up records
- Synchronization logs
- User authentication
- Dashboard analytics

The selected database solution must also support offline operation and automatic synchronization.

---

# 3. Selected Database Architecture

CampSync uses a hybrid database architecture.

### Primary Database

**PostgreSQL**

Used for:

- Patient records
- Equipment inventory
- NGO information
- Hospital referrals
- Reports
- Dashboard analytics
- User accounts

---

### Local Offline Database

**IndexedDB**

Used for:

- Offline patient registration
- Offline medical records
- Temporary inventory updates
- Pending synchronization queue

When internet connectivity is restored, data stored in IndexedDB is synchronized with PostgreSQL.

---

# 4. Why PostgreSQL?

PostgreSQL is selected as the primary database because it is an advanced, open-source relational database management system (RDBMS).

### Advantages

- Open source
- ACID compliant
- High reliability
- Excellent data integrity
- Supports complex relationships
- JSON support
- Strong security
- Scalable for future growth

PostgreSQL is well suited for storing structured healthcare data that requires consistency and reliability.

---

# 5. Why IndexedDB?

IndexedDB is a browser-based NoSQL database that supports offline storage.

### Advantages

- Works without internet
- Large storage capacity
- Fast local search
- Structured object storage
- Native browser support
- Persistent storage

IndexedDB enables volunteers to continue working during healthcare camps even when internet connectivity is unavailable.

---

# 6. SQL vs NoSQL

CampSync combines both SQL and NoSQL technologies to leverage the strengths of each.

| Feature | PostgreSQL (SQL) | IndexedDB (NoSQL) |
|---------|------------------|-------------------|
| Data Type | Structured | Semi-Structured |
| Relationships | Strong | Limited |
| Offline Support | No | Yes |
| ACID Transactions | Yes | Limited |
| Scalability | High | Browser-Based |
| Primary Use | Central Database | Offline Storage |

This hybrid approach ensures reliability while maintaining offline capability.

---

# 7. Database Entities

The major entities in CampSync include:

- Patient
- Volunteer
- NGO Administrator
- Healthcare Camp
- Medical Examination
- Equipment
- Equipment Assignment
- Hospital Referral
- Follow-up Record
- Synchronization Log
- User Account

These entities will later be represented in the Entity Relationship (ER) Diagram.

---

# 8. Data Relationships

Examples of relationships include:

- One volunteer registers many patients.
- One patient can have multiple medical examinations.
- One healthcare camp serves many patients.
- One patient may receive multiple equipment items over time.
- One referral belongs to one patient.
- One NGO administrator manages multiple healthcare camps.

These relationships help maintain consistency and avoid duplicate records.

---

# 9. Synchronization Strategy

CampSync follows an offline-first synchronization model.

### Step 1

The volunteer registers patient information while offline.

↓

### Step 2

Data is stored locally in IndexedDB.

↓

### Step 3

The Service Worker detects internet availability.

↓

### Step 4

Pending records are sent to the backend through the synchronization API.

↓

### Step 5

The backend validates the received data.

↓

### Step 6

Records are stored permanently in PostgreSQL.

↓

### Step 7

Synchronization status is updated on the volunteer's device.

This strategy minimizes data loss and ensures uninterrupted healthcare operations.

---

# 10. Conflict Resolution

Synchronization conflicts may occur when multiple users modify the same record.

CampSync will address these conflicts by:

- Assigning unique identifiers (UUIDs)
- Maintaining timestamps
- Recording synchronization history
- Validating data on the server
- Alerting administrators when manual review is required

This approach improves data consistency and prevents accidental overwriting.

---

# 11. Data Security

Healthcare data is sensitive and must be protected.

CampSync incorporates the following security measures:

- User authentication
- Role-based access control
- HTTPS communication
- JWT authentication
- Password hashing
- Secure database access
- Regular backups

These measures help maintain patient confidentiality and data integrity.

---

# 12. Backup and Recovery

Regular database backups are necessary to prevent data loss.

The backup strategy includes:

- Automated PostgreSQL backups
- Transaction logging
- Periodic cloud backups
- Recovery testing
- Version-controlled database scripts

This ensures that patient records and inventory data can be restored if required.

---

# 13. Future Scalability

The database architecture supports future enhancements such as:

- AI-based disease prediction
- Government health system integration
- Multi-NGO support
- Multi-language support
- GIS-based camp mapping
- Predictive inventory management

The modular database design allows these features to be incorporated without major structural changes.

---

# 14. Conclusion

The hybrid database architecture of PostgreSQL and IndexedDB provides an effective solution for CampSync. PostgreSQL ensures reliable centralized data management, while IndexedDB enables uninterrupted offline operation during healthcare camps.

This design fulfills the project's requirements for reliability, scalability, security, and offline-first functionality.

---

# References

This database analysis is supported by the literature reviewed during the research phase, particularly:

- Paper 3 – Offline-first healthcare applications
- Paper 4 – Progressive Web Application architecture
- Paper 5 – IndexedDB performance evaluation
- Paper 6 – Offline synchronization techniques
- Paper 7 – Digital healthcare registration systems
- Paper 9 – Healthcare information management systems
- Paper 15 – Medical inventory systems
- Paper 17 – Secure healthcare databases
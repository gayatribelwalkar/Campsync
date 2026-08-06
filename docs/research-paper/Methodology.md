# IV. Methodology
The development of CampSync follows a systematic Software Engineering approach to ensure that the proposed system is reliable, scalable, and suitable for real-world NGO healthcare camps. The methodology adopted for this research consists of requirement analysis, literature review, system design, implementation planning, and evaluation.

## A. Requirement Analysis
The first phase involved identifying the operational challenges faced by NGOs while conducting healthcare camps. Information was gathered through problem analysis, existing literature, and observations of common healthcare camp workflows. The primary functional requirements identified include offline patient registration, medicine inventory management, hospital referral tracking, administrator monitoring, and patient follow-up. Non-functional requirements such as reliability, security, usability, scalability, and offline accessibility were also considered during system planning.

---

## B. Literature Review and Research Gap Analysis

A comprehensive review of twenty-two research papers was conducted to understand the current state of healthcare management systems, Progressive Web Applications, Electronic Health Records, inventory management, and offline synchronization techniques. Each paper was analyzed to identify the technologies used, methodologies adopted, strengths, limitations, and potential research gaps.

The literature review revealed that most existing systems focus on individual functionalities such as patient record management, medicine inventory, or telemedicine. Very few studies provide an integrated solution specifically designed for NGO healthcare camps operating in low-bandwidth environments. These findings formed the foundation for designing the proposed CampSync system.

---

## C. System Design

Based on the identified research gaps and project requirements, the CampSync architecture was designed using an offline-first approach. The system follows a layered architecture consisting of presentation, application, and data layers.

The presentation layer provides responsive user interfaces for volunteers and administrators. The application layer manages business logic, authentication, synchronization, and report generation. The data layer utilizes IndexedDB for offline local storage and PostgreSQL for centralized cloud storage. Automatic synchronization ensures that locally stored data is uploaded whenever internet connectivity becomes available.

---

## D. Technology Selection

The technologies used for developing CampSync were selected based on scalability, ease of development, offline capabilities, and community support.

| Component | Technology |
|-----------|------------|
| Frontend | HTML5, CSS3, JavaScript |
| Backend | Node.js, Express.js |
| Database | PostgreSQL |
| Offline Storage | IndexedDB |
| Offline Support | Progressive Web Application (PWA), Service Workers |
| Version Control | Git & GitHub |
| Documentation | Markdown, Microsoft Word |
| Reference Management | Zotero |

These technologies collectively provide a robust environment for developing an offline-first healthcare management system.

---

## E. System Development Process

CampSync follows the Agile Software Development methodology. The project is divided into multiple incremental phases, allowing continuous improvement throughout development.

The development process includes:

1. Requirement Analysis
2. Literature Review
3. System Study
4. Feasibility Analysis
5. Software Requirement Specification (SRS)
6. System Design
7. Database Design
8. Frontend Development
9. Backend Development
10. Testing and Validation
11. Documentation
12. Final Deployment

This iterative development approach allows changes to be incorporated throughout the project while maintaining documentation and version control.

---

## F. Expected Evaluation

As the project is currently under development, the evaluation will focus on functional validation rather than performance benchmarking. The proposed system will be assessed based on successful offline patient registration, synchronization accuracy, inventory management, referral generation, administrator dashboard functionality, and overall usability.

Future evaluation will also compare CampSync with existing healthcare management systems in terms of offline capability, operational efficiency, scalability, and user experience.
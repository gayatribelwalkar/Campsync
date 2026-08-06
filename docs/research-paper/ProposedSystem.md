# III. Proposed System
## A. Existing System

Existing healthcare management systems are primarily designed for hospitals, clinics, or urban healthcare centers where continuous internet connectivity is available. Most systems focus on a single aspect of healthcare management, such as electronic health records, medicine inventory, patient registration, telemedicine, or disease surveillance. Although these systems have significantly improved healthcare digitization, they exhibit several limitations when deployed in temporary NGO healthcare camps conducted in rural and underserved areas.

Many existing solutions rely heavily on cloud-based databases, making them unsuitable for locations with poor or unstable internet connectivity. During healthcare camps, volunteers often experience interrupted network access, leading to incomplete patient registration, delayed synchronization, duplicate records, and inefficient inventory management. Furthermore, current systems rarely integrate patient registration, medicine inventory, hospital referral management, volunteer coordination, and administrative reporting into a single platform. These limitations reduce operational efficiency and create additional workload for healthcare workers.

---

## B. Proposed CampSync System

CampSync is proposed as a comprehensive offline-first healthcare and medical inventory management system specifically developed for NGO-organized healthcare camps. The system is designed as a Progressive Web Application (PWA), enabling field volunteers to continue healthcare operations regardless of internet availability.

The proposed system allows volunteers to register patients, maintain digital medical records, record vital information, manage medicines and donated medical equipment, and generate referrals directly from their mobile devices or laptops. All information is stored locally using IndexedDB while the device remains offline. Once internet connectivity becomes available, the synchronization engine securely transfers local records to the centralized PostgreSQL database.

CampSync also provides an administrator dashboard that enables NGO officials to monitor healthcare camps, allocate inventory, generate analytical reports, track patient referrals, and evaluate healthcare outcomes. In addition, patients receive follow-up notifications and feedback requests through WhatsApp, improving post-camp communication and healthcare continuity.

By integrating offline functionality, patient management, inventory management, synchronization services, and administrative monitoring into one unified platform, CampSync addresses several research gaps identified in existing healthcare management systems.

---

## C. System Architecture

The proposed architecture follows a layered client-server model designed to support reliable offline-first operations.

The presentation layer consists of a Progressive Web Application (PWA) that provides responsive interfaces for volunteers and administrators. The application uses Service Workers to cache essential resources and enable uninterrupted operation without internet connectivity.

The application layer contains backend services developed using Node.js and Express.js, which handle business logic, authentication, synchronization, report generation, and communication between the client application and centralized database.

The data layer consists of IndexedDB for offline local storage and PostgreSQL for centralized cloud storage. A synchronization mechanism ensures that locally stored records are securely transferred to the central database whenever internet connectivity is restored.

---

## D. System Development

The development of CampSync follows the Agile Software Development methodology. Project development is divided into incremental phases including requirement analysis, literature review, system study, system design, database design, frontend development, backend development, testing, deployment, and documentation.

The frontend is developed using HTML5, CSS3, JavaScript, and Progressive Web Application technologies. Backend services are implemented using Node.js and Express.js, while PostgreSQL serves as the centralized relational database. IndexedDB is utilized for offline data storage, and Service Workers enable caching and synchronization functionality required for offline-first operations.

Version control is maintained using Git and GitHub, enabling continuous documentation, collaboration, and project tracking throughout the development lifecycle.

---

## E. Advantages of the Proposed System

The proposed CampSync system offers several advantages over existing healthcare management systems.

- Supports complete offline functionality using Progressive Web Application technology.
- Enables uninterrupted patient registration during internet outages.
- Provides centralized synchronization of patient records after connectivity restoration.
- Integrates patient registration, medicine inventory, donated equipment tracking, and hospital referrals into a unified platform.
- Reduces paperwork and duplicate data entry.
- Improves healthcare camp efficiency through digital workflow automation.
- Supports administrator dashboards for monitoring healthcare camps and generating reports.
- Facilitates patient follow-up using WhatsApp notifications.
- Provides scalable architecture suitable for deployment across multiple NGO healthcare camps.
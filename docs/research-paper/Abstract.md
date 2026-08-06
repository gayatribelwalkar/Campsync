# Abstract


Healthcare camps organized by Non-Governmental Organizations (NGOs) play a significant role in providing medical services to underserved and rural communities. However, these camps often rely on paper-based records or internet-dependent applications, making patient registration, medical record management, inventory tracking, and follow-up activities inefficient in locations with poor or unstable network connectivity.

This research proposes **CampSync**, an offline-first healthcare and medical inventory management system designed specifically for NGO health camps. The proposed system utilizes a Progressive Web Application (PWA) architecture with IndexedDB for local data storage, allowing field volunteers to register patients, record medical information, and manage medicine inventory without requiring continuous internet access. Once connectivity is restored, the system securely synchronizes locally stored data with a centralized cloud database, ensuring consistency and preventing data loss.

A comprehensive literature review of twenty-two research papers on offline-first applications, healthcare information systems, electronic health records, mobile health technologies, inventory management, and Progressive Web Applications was conducted to identify existing limitations and research gaps. Based on these findings, CampSync integrates offline data synchronization, patient management, medicine inventory monitoring, NGO administration, and follow-up management into a unified platform.

The proposed system aims to improve operational efficiency, reduce manual errors, enhance data availability in low-bandwidth environments, and support healthcare workers in delivering reliable medical services during outreach programs. This paper presents the system architecture, methodology, literature analysis, and the expected benefits of implementing CampSync in real-world healthcare camps.

**Keywords:** Offline-First Application, Progressive Web Application (PWA), Healthcare Management, NGO Health Camps, IndexedDB, Patient Management System, Medical Inventory Management, FastAPI, MongoDB.
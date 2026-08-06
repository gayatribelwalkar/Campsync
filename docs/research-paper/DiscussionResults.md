# V. Discussion and Expected Results

Since CampSync is currently under development, the results presented in this paper are based on the proposed system architecture, literature analysis, and expected system performance rather than completed implementation. The literature review indicates that existing healthcare management systems successfully address individual challenges such as electronic health records, medicine inventory, offline synchronization, or hospital management. However, very few systems provide a unified solution specifically designed for NGO healthcare camps operating in remote and low-bandwidth environments.

The proposed CampSync system is expected to overcome these limitations by integrating offline patient registration, medical inventory management, hospital referral tracking, administrator monitoring, and patient follow-up within a single Progressive Web Application. The use of IndexedDB enables uninterrupted data collection even without internet connectivity, while synchronization with the centralized PostgreSQL database ensures data consistency after network restoration.

Compared with traditional paper-based healthcare camp management, CampSync is expected to reduce manual documentation, minimize duplicate patient records, improve inventory tracking, and simplify report generation. The administrator dashboard will provide centralized monitoring of healthcare activities, enabling NGOs to make informed operational decisions and allocate medical resources more efficiently.

Table 1 summarizes the expected comparison between existing healthcare management systems and the proposed CampSync platform.

| Feature | Existing Systems | CampSync |
|---------|------------------|-----------|
| Offline Patient Registration | Limited | Yes |
| Progressive Web Application | Partial | Yes |
| IndexedDB Local Storage | Limited | Yes |
| Medical Inventory Management | Partial | Yes |
| Hospital Referral Tracking | Limited | Yes |
| NGO Healthcare Camp Support | Limited | Yes |
| Administrator Dashboard | Partial | Yes |
| WhatsApp Patient Follow-up | Rare | Yes |
| Unified Healthcare Workflow | No | Yes |

Based on the literature review and system design, CampSync is expected to improve operational efficiency, reduce paperwork, enhance data availability in low-connectivity environments, and support reliable healthcare delivery during NGO healthcare camps. Future implementation and field testing will be conducted to validate these expected outcomes.
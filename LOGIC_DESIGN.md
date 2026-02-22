**AARUDHRA: System Logic & Architectural Decisions**
* **Author: CHANDANA V** – Idea Provider & System Architect
* 
**1. Problem Statement & Conceptualization**
*In rural India, emergency response is often delayed due to inaccurate mapping and fragmented contact databases. I conceptualized AARUDHRA to act as a localized "Command Center" on a mobile device, ensuring that even with low technical literacy, a user can trigger a high-speed response.

**2. API Selection: Why OpenStreetMap?**
The team implemented the OpenStreetMap (OSM) API based on my strategic requirements:
*  Offline Capability: Crucial for rural areas with intermittent 4G/5G connectivity.
*  Resource Efficiency: OSM handles tiles efficiently, reducing the app's memory footprint on entry-level smartphones.
*  Open Source: Aligns with the conference theme of "Sustainable Technology.

**3. Search & Sort Logic Architecture**
  To achieve a 30% reduction in retrieval time, I designed the data flow as follows:
*   Priority Ranking: Contacts are indexed by proximity and "Service Type" (e.g., Ambulance) using a custom indexing method.
*   Modular Logic: Structured the system into four core modules: First Aid, Hospital Locator, Chatbot, and Health Monitor.
  
  **4. Conference Defense & Q&A**
   During the ICISTEEH-26 presentation, I served as the primary respondent for the panel. Key queries I addressed included:
    How does this help rural populations who may already be familiar with local emergencies like snake bites?
* **Response:** While local knowledge exists, statistics show rising mortality due to the lack of immediate medical coordination. AARUDHRA transforms "local awareness" into "digitally triggered action." It provides standardized first-aid steps for snake bites (including audio guidance) while simultaneously locating the nearest specialized facility, bridging the critical gap between incident and professional care.

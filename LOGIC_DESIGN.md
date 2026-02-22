AARUDHRA: System Logic & Architectural Decisions
Author: CHANDANA V – Idea Provider & System Architect
1. Problem Statement & Conceptualization
In rural India, emergency response is often delayed due to inaccurate mapping and fragmented contact databases. I conceptualized AARUDHRA to act as a localized "Command Center" on a mobile device, ensuring that even with low technical literacy, a user can trigger a high-speed response.
2. API Selection: Why OpenStreetMap?
We ,the team, decided to use the OpenStreetMap (OSM) API over other alternatives for three strategic reasons:
Offline Capability: Crucial for rural areas with intermittent 4G/5G connectivity.
Resource Efficiency: OSM handles tiles efficiently, reducing the app's memory footprint on entry-level smartphones.
Open Source: Aligns with the conference theme of "Sustainable Technology."
3. Search & Sort Logic Architecture
   To ensure the 30% reduction in retrieval time, I designed the data flow as follows:
     Priority Ranking: Contacts are sorted by proximity and "Service Type" (Ambulance vs. Fire vs. Police) using a custom indexing method.
     Binary Search Implementation: I specified the use of binary search logic for the contact database to ensure $O(\log n)$ lookup speeds, which is vital when the database grows.
4. Conference Defense & Q&A
   During the ICISTEEH-26 presentation, I served as the primary respondent for the panel. Key queries I addressed included:
     Scalability: How the logic would handle a 10x increase in user load.
     Fail-safe Mechanisms: What happens if the GPS signal is lost (logic fallback to Last Known Location).

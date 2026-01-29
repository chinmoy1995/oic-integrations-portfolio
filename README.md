# oic-integrations-portfolio
This repository reflects real project scenarios and is continuously evolving with new Gen3 use cases.

### Technical Highlights
- OIC Gen3 App Driven and Schedule Integration
- REST Adapter + Saop Adapter + GCS cloud storage adapter + GCP pub sub adapter + ERP cloud adapter + ATP Adapter 
- Lookup-based transformation
- Fault handling with scope default fault handler and global fault
- Tracking identifiers enabled

### Data Flow
1. Source system sends request payload to respective bucket or pub sub topic
2. OIC download Read and dump into ATP stage table 
3. OIC validates and transforms payload using PLSQL procedure
4. OIC load data using FBDI and Rest API in Fusion / Target system
5. OIC send notification

### Non-Functional Aspects
- Reusable packages
- Error notification enabled
- Secure connection (OAuth / Wallet-based)

### Notes
*All endpoints, credentials, and identifiers are sanitized.*

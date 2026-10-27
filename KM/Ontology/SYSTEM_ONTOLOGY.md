# Enterprise System & Knowledge Ontology

## 1. Core Entity Types
* **Systems & Applications:** Software platforms, enterprise tools, databases, and microservices.
* **Data Objects:** Core master data entities exchanged between platforms (e.g., User Profile, Inventory Record, Financial Ledger).
* **Business Processes:** Operational workflows executed by human actors or automated jobs (e.g., Data Ingestion, Batch Sync, Reporting).
* **Roles & Owners:** Stakeholders responsible for governance, maintenance, or data consumption (e.g., System Owner, Data Steward, Business Analyst).

---

## 2. Generic Semantic Relationship Map

```text
[System of Record] --(IS_PRIMARY_SOURCE_FOR)--> [Master Data Object]
[System of Record] --(FEEDS_DATA_TO)----------> [Downstream Application]
[Downstream App]  --(GENERATES)-------------> [Transaction Logs / Artifacts]
[Data Steward]     --(GOVERNS)----------------> [Master Data Object]
[Business Process] --(DEPENDS_ON)-------------> [System of Record]

# CalSAAS — California Statewide Assignment Accountability System

CalSAAS is the system used to **annually monitor certificated educator assignments** in California.

Source: https://www.ctc.ca.gov/employers/calsaas/ (downloaded 2026-08-28)

---

## 1. What CalSAAS Does

CalSAAS works by **comparing**:

- The **CDE's CALPADS** assignment data (California Longitudinal Pupil Achievement Data System), and
- The **Commission's credential authorization data**,

...matched by each educator's **California Statewide Educator Identifier (SEID)**.

Through this comparison, the system identifies **questionable assignments** ("exceptions") and gives LEAs and County Offices of Education (COEs) an opportunity to address anomalies and **correct misassignments**.

---

## 2. Key Components

- **CalSAAS Login** — web portal for MAs and LEAs.
- **CalSAAS FAQs** — frequently asked questions.
- **Annual System Enhancements** — yearly updates.
- **CalSAAS Training** — ~60-minute training module.
- **Video Tutorials** — Managing Users, Exception Overview Process, User Workload, Notifications.
- **CalSAAS Glossary of Terms**.
- **Reporting Substitute Assignments in CalSAAS**.
- **Troubleshooting in CalSAAS**.
- **Specific Exception Information**.
- **CalSAAS User Manual** — covers Overview, CALPADS Reporting, Users, Exceptions, Status, Determinations, Charter Schools, Reports, MA Reported Misassignments, TPSL List.

---

## 3. Appropriate Credential Authorizations for CALPADS Coding

The Commission publishes reference documents mapping CALPADS codes to appropriate credentials:

| Reference | Purpose |
|-----------|---------|
| **Course Assignment Handout** | How to determine course content and the appropriate credential |
| **Appropriate Credentials for CALPADS State Course Codes** | Which credentials authorize each CALPADS course code |
| **Appropriate Credentials for Special Education Disability Categories** | Which credentials authorize each special-ed disability category |
| **Appropriate Credentials for English Learner Services** | Which credentials authorize each EL service code |
| **Appropriate Credentials for Non Classroom Based Assignments** | Which credentials authorize non-classroom-based (service) assignments |

These are the authoritative mappings behind the `data/calpads-course-codes.csv` and `data/credential-authorizations.csv` files in this repo.

---

## 4. Exception Determination Process

For each reported assignment, CalSAAS determines:

1. Does the educator hold the appropriate authorization for the assignment?
   - Valid on the **census date** → **Appropriate Assignment**.
   - Not valid on census date but issued before monitoring → **Corrected Misassignment**.
   - Services/authorization appropriate but an exception was generated → **CALPADS Error**.
2. If the educator does **not** hold the appropriate authorization:
   - → **Misassignment** or **Vacancy** (if a substitute was reported in the assignment).

---

## 5. Relationship to CALPADS

- **Starting in the 2019-20 school year**, the Commission uses **CALPADS course assignments** for monitoring purposes.
- LEAs must **accurately report all educator and service provider assignments** in CALPADS.
- CALPADS course assignments should be selected **based entirely on the content of the course or the nature of the position**, after the course content is determined.
- For help determining the appropriate CALPADS course code, contact the CDE's CALPADS Operations Office at **calpads@cde.ca.gov**.

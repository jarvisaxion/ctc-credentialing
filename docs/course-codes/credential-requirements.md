# Credential Requirements by Course

This document provides a structured breakdown of the **credential requirements** for CALPADS course codes, organized by subject area. It answers the question: **"What credential does a teacher need to be properly credentialed for this class?"**

The data is derived from the CTC's "Appropriate Credentials for CALPADS Course Codes" table (`raw/calpads-course-codes.csv`).

> **Source:** CTC "Appropriate Credentials for CALPADS Course Codes" — https://www.ctc.ca.gov/employers/calsaas/calpads-course-codes/ (raw: `raw/calpads-course-codes.csv`, `raw/calpads-course-codes-data.txt`). Downloaded 2026-08-28.

---

## General Education / Self-Contained

> **Source:** `raw/calpads-course-codes.csv` (course code `1000`).

| Course Code | Course Title | Required Credential |
|-------------|--------------|---------------------|
| `1000` | Self-Contained Class | **Multiple Subject** |

---

## Career Technical Education (CTE) — By Industry Sector

> **Source:** `raw/calpads-course-codes.csv` (CTE course codes `7000`+); Title 5 §80004(c) flexibility per CTC assignment resources.

CTE courses are authorized by a **CTE credential in the relevant industry sector**. Many also allow a related **Single Subject** credential at the employing agency's discretion (Title 5 §80004(c)).

### Agriculture and Natural Resources (codes `7100`–`7172`)
- **Full authorization:** CTE: Agriculture and Natural Resources
- **Also authorized (discretionary):** Single Subject: Agriculture

### Arts, Media, and Entertainment (codes `7200`–`7263`)
- **Full authorization:** CTE: Arts, Media, and Entertainment
- **Also authorized (discretionary):** Single Subject: Industrial and Technology Education

### Building and Construction Trades (codes `7300`+)
- **Full authorization:** CTE: Building and Construction Trades
- **Also authorized (discretionary):** Single Subject: Industrial and Technology Education

### Education, Child Development, and Family Services (code `7001`)
- **Full authorization:** CTE: Education, Child Development, and Family Services
- **Also authorized (discretionary):** Single Subject: Home Economics

### Other CTE Sectors

> **Source:** `raw/calpads-course-codes.csv` (CTE course codes `7000`+).

- **Business and Finance:** CTE: Business and Finance
- **Health Science and Medical Technology:** CTE: Health Science and Medical Technology
- **Information and Communication Technology:** CTE: Information and Communication Technology
- **Engineering and Architecture:** CTE: Engineering and Architecture
- **Manufacturing and Product Development:** CTE: Manufacturing and Product Development
- **Marketing, Sales, and Service:** CTE: Marketing, Sales, and Service
- **Public Service:** CTE: Public Service
- **Transportation:** CTE: Transportation
- **Energy, Environment, and Utilities:** CTE: Energy, Environment, and Utilities
- **Hospitality, Tourism, and Recreation:** CTE: Hospitality, Tourism, and Recreation
- **Fashion and Interior Design:** CTE: Fashion and Interior Design

---

## Departmentalized Academic Subjects

> **Source:** `raw/calpads-course-codes.csv` (academic course codes); CTC authorization statements for Single Subject credentials.

Academic courses are authorized by the corresponding **Single Subject** credential.

| Broad Subject | Required Credential |
|---------------|---------------------|
| English | Single Subject: English |
| Mathematics | Single Subject: Mathematics |
| Science | Single Subject: Science (Biology, Chemistry, Physics, etc.) |
| Social Science | Single Subject: History–Social Science |
| World Languages | Single Subject: World Languages (specific language) |
| Art / Visual Art | Single Subject: Art |
| Music | Single Subject: Music |
| Theatre / Dance | Single Subject: Theatre / Dance |
| Physical Education | Single Subject: Physical Education |
| Health | Single Subject: Health Science (or related) |
| Computer Science | Single Subject: Computer Science (or related) |
| Digital Literacy | Single Subject: Computer Science / Business |
| Driver Education | Designated Subjects / related |

---

## Special Education

> **Source:** `raw/calpads-course-codes.csv` (special education course codes); CTC Authorization Sort Table (`raw/auth-sort-data.txt`).

Special education courses are authorized by **Education Specialist** credentials.

| Broad Subject | Required Credential |
|---------------|---------------------|
| Special Education Support | Education Specialist Instruction Credential (relevant support-need category) |
| Adapted Physical Education | Education Specialist + Adapted PE Added Authorization |

---

## Electives & Other

> **Source:** `raw/calpads-course-codes.csv` (elective/other course codes).

| Broad Subject | Required Credential |
|---------------|---------------------|
| Elective | Varies by course content |
| ROTC | Designated Subjects / military-related |
| Librarian | Teacher Librarian Services Credential |
| Resource Services | Education Specialist / Resource Specialist |
| Study Hall | Varies (often no specific credential) |

---

## Important Notes

> **Source:** CTC "Appropriate Credentials for CALPADS Course Codes" — https://www.ctc.ca.gov/employers/calsaas/calpads-course-codes/; CTC assignment resources (Title 5 §80004(c)).

1. **"Full Authorization"** means the credential listed fully authorizes teaching the course — the teacher is properly credentialed.
2. **Title 5 §80004(c) flexibility** — for many CTE courses, a related Single Subject credential may be used at the **employing agency's discretion**. This is not automatic; the district must choose to apply it.
3. **Self-contained vs. departmentalized** — course code `1000` (self-contained) requires Multiple Subject; departmentalized academic courses require Single Subject.
4. **Always verify** against the current CTC "Appropriate Credentials for CALPADS Course Codes" table, as course codes and requirements are updated.

---

## Full Machine-Readable Data

> **Source:** `data/calpads-course-codes.csv` (parsed from `raw/calpads-course-codes.csv`).

See `data/calpads-course-codes.csv` for the complete table of all 681 course codes with their credential requirements.

---

## Sources

- CTC Appropriate Credentials for CALPADS Course Codes: https://www.ctc.ca.gov/employers/calsaas/calpads-course-codes/
- CTC Credential Type and Authorization Statements: https://www.ctc.ca.gov/employers/tools-and-resources/credential-type-and-authorization-statements/
- CTC Assignment Resources: https://www.ctc.ca.gov/employers/assignment-resources/
- Raw data: `raw/calpads-course-codes.csv`, `raw/calpads-course-codes-data.txt`, `raw/credential-type-data.txt`, `raw/auth-sort-data.txt`

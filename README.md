# California K-12 Teacher Credentialing & Course Code Reference

A comprehensive, machine-readable reference for **California teacher credentialing and authorization**, and the **CALPADS course codes** that determine which credentials properly authorize a teacher to teach each course.

This repository consolidates and documents the official data published by the **California Commission on Teacher Credentialing (CTC)** and the **California Department of Education (CDE)**.

---

## What This Repo Contains

| Area | Description | Primary Source |
|------|-------------|----------------|
| **Credential types** | Every credential, permit, certificate, and authorization the CTC issues, with codes and names | CTC credentialing data files (T01) |
| **Authorization statements** | What each credential authorizes the holder to do (grade levels, subjects, services) | CTC credentialing data files (T06) |
| **Special education authorizations** | Which disability categories each special-ed authorization covers | CTC Authorization Sort Table |
| **CALPADS course codes** | Every course code, its subject/setting, and the credentials that fully authorize teaching it | CTC "Appropriate Credentials for CALPADS Course Codes" |
| **Assignment determination & monitoring** | How California determines whether a teacher is appropriately assigned, the hiring hierarchy, LAOs, emergency permits, EL authorizations, CalSAAS monitoring | CTC Assignment Resources site |

---

## Repository Layout

```
ctc-credentialing/
├── README.md                     # This file
├── docs/
│   ├── credentials/
│   │   ├── credential-types.md   # All credential types, codes, and what they authorize
│   │   ├── single-subject.md     # Single Subject Teaching Credential details
│   │   ├── multiple-subject.md   # Multiple Subject Teaching Credential details
│   │   ├── education-specialist.md # Special education credentials & authorizations
│   │   ├── designated-subjects.md  # CTE / designated subjects credentials
│   │   ├── permits.md            # Permits, certificates, and authorizations
│   │   └── special-ed-authorizations.md # Disability-category authorization matrix
│   ├── course-codes/
│   │   ├── calpads-course-codes.md  # Full CALPADS course code reference
│   │   └── credential-requirements.md # How credential requirements map to courses
│   └── assignment/
│       ├── assignment-monitoring.md  # How assignments are determined & monitored
│       ├── calsaas.md                # CalSAAS monitoring system
│       └── credential-types-history.md # History of teaching credentials
├── data/
│   ├── calpads-course-codes.csv  # Cleaned, machine-readable course code table
│   └── credential-types.csv      # Cleaned credential type table
├── raw/                          # Original downloaded reference data (unchanged)
│   ├── T01FILE.txt ... T22FILE.txt  # CTC credentialing data table files
│   ├── calpads-course-codes.csv     # Raw course code export
│   ├── auth-sort.txt                # Special ed authorization sort table
│   └── ...                          # HTML/PDF/text snapshots of source pages
└── scripts/
    └── (parsing/cleaning scripts)
```

---

## Key Concepts

### 1. Credential Types (What a teacher can hold)

California issues credentials, permits, certificates, and authorizations through the CTC. The main **teaching credentials** are:

- **Multiple Subject Teaching Credential** — authorizes teaching in self-contained classrooms (typically elementary, TK–6, and some middle school).
- **Single Subject Teaching Credential** — authorizes teaching a specific subject (e.g., Mathematics, English, Science) in departmentalized settings (typically middle/high school, grades 7–12).
- **Education Specialist Instruction Credential** — authorizes teaching students with disabilities (special education), with specific disability-area authorizations.
- **Designated Subjects Career Technical Education (CTE) Teaching Credential** — authorizes teaching career technical education courses in specific industry sectors.
- **Specialist Instruction Credentials** — for specialized areas (Agriculture, Bilingual, Early Childhood, Gifted, Health Science, Mathematics, Reading, Special Education).

Plus **permits** (e.g., substitute, short-term staff, provisional intern), **certificates** (e.g., Bilingual Certificate of Competence, Certificate of Clearance), and **added authorizations** (e.g., Reading and Literacy Added Authorization, Bilingual Authorization).

### 2. Authorization (What a credential lets a teacher do)

Each credential's **authorization statement** (T06 data) spells out:
- **Grade levels** (e.g., "grades twelve and below, including preschool, and classes organized primarily for adults")
- **Subjects** (e.g., "mathematics content typically included in curriculum guidelines and textbooks up to and including Algebra I")
- **Services** (e.g., "develop and coordinate mathematics curriculum; coach mathematics teachers")

### 3. CALPADS Course Codes (What course a teacher can be assigned)

CALPADS (California Longitudinal Pupil Achievement Data System) assigns a **course code** to every course a school offers. The CTC publishes the **"Appropriate Credentials for CALPADS Course Codes"** table, which lists, for each course code, the credential(s) that provide **full authorization** to teach that course.

**This is the critical link:** a teacher is "properly credentialed" for a class when the credential they hold appears in the "Credentials Authorizing Course" column for that course's CALPADS code.

---

## How to Use This Reference

**To determine if a teacher is properly credentialed for a course:**

1. Find the course's **CALPADS course code** (from the school's master schedule / CALPADS submission).
2. Look up that code in `data/calpads-course-codes.csv` or `docs/course-codes/calpads-course-codes.md`.
3. Read the **"Credentials Authorizing Course"** column — this lists the credential(s) that fully authorize teaching that course.
4. Compare against the teacher's actual credential(s) and their authorization statements.

**Example:** Course code `1000` (Self-Contained Class) requires a **Multiple Subject** credential. A teacher holding only a Single Subject credential in Mathematics would **not** be fully authorized for a self-contained elementary class.

---

## Source Data & Provenance

All reference data was downloaded from the official CTC website on **2026-08-28**:

1. **Shared Credential Info** — https://www.ctc.ca.gov/employers/tools-and-resources/shared-cred-info/
   - The T01–T22 credentialing data table files (replaced weekly every Thursday).
2. **Credential Type and Authorization Statements** — https://www.ctc.ca.gov/employers/tools-and-resources/credential-type-and-authorization-statements/
   - The full list of credential types and their authorization statements.
3. **Tools and Resources** — https://www.ctc.ca.gov/employers/tools-and-resources/
   - Index of employer-facing credentialing tools.
4. **Appropriate Credentials for CALPADS Course Codes** — https://www.ctc.ca.gov/employers/calsaas/calpads-course-codes/
   - The course-code-to-credential mapping table.
5. **Assignment Resources** — https://www.ctc.ca.gov/employers/assignment-resources/
   - Assignment determination & monitoring, hiring hierarchy, LAOs, emergency permits, EL authorizations, CalSAAS, charter school assignments, and 7 training module handouts (all preserved in `raw/assignment-resources/`).

The `raw/` directory contains the original, unmodified downloads for provenance and verification.

---

## Disclaimer

This repository is a **reference compilation** of publicly available CTC/CDE data. It is provided for informational purposes. For official determinations of a teacher's credentialing status, always consult the **California Commission on Teacher Credentialing** directly (https://www.ctc.ca.gov) or the employing agency's credential analyst. Credentialing rules change; verify against current CTC guidance before making assignment decisions.

# CALPADS Course Codes & Credential Requirements

This document is the reference for **California state course codes** (CALPADS) and the **credential requirements** for each course — i.e., what credential a teacher must hold to be considered **properly credentialed** for a given class.

The data comes from the CTC's **"Appropriate Credentials for CALPADS Course Codes"** table.

---

## What Is CALPADS?

**CALPADS** (California Longitudinal Pupil Achievement Data System) is California's statewide data system for tracking pupil achievement. Every course a school offers is assigned a **course code** in CALPADS. The course code identifies the course's subject area and setting.

The CTC publishes, for each course code, the **credential(s) that provide full authorization** to teach that course. This is the authoritative mapping for determining whether a teacher is properly credentialed for a class.

---

## How to Read the Course Code Table

Each course code entry has these fields:

| Field | Description |
|-------|-------------|
| **Course Code** | The CALPADS course code (e.g., `1000`, `7100`) |
| **Course Title** | The name of the course |
| **Broad Subject** | The subject area (e.g., Mathematics, Science, CTE sector) |
| **Setting** | The instructional setting (e.g., General Education, Career Technical Education, Special Education) |
| **Credentials Authorizing Course** | The credential(s) that provide **full authorization** to teach this course |
| **Notes** | Additional notes (e.g., Title 5 §80004(c) flexibility) |

---

## The Main Course Code Ranges

CALPADS course codes are organized into ranges by subject/setting:

| Code Range | Subject / Setting |
|------------|-------------------|
| `1000` | Self-Contained Class (General Education) |
| `7000`–`7999` | Career Technical Education (CTE) courses |
| Various | Departmentalized academic subjects (English, Math, Science, Social Science, World Languages, etc.) |
| Various | Special Education Support |
| Various | Electives, Physical Education, Art, Music, etc. |

---

## Credential Requirement Patterns

The "Credentials Authorizing Course" column follows recognizable patterns:

### 1. Self-Contained (Elementary)
- **Course code `1000`** (Self-Contained Class) requires a **Multiple Subject** credential.
- This is the standard for elementary self-contained classrooms.

### 2. Career Technical Education (CTE)
- CTE courses (codes `7000`+) are authorized by a **CTE credential in the relevant industry sector**.
- Many also allow a **Single Subject** credential in a related area (Agriculture, Business, Home Economics, Industrial and Technology Education) at the employing agency's discretion (Title 5 §80004(c)).

### 3. Departmentalized Academic Subjects
- Academic courses (English, Math, Science, etc.) are authorized by the corresponding **Single Subject** credential.

### 4. Special Education
- Special education courses are authorized by **Education Specialist** credentials.

---

## Full Course Code Table

The complete, machine-readable course code table is in:

- **`data/calpads-course-codes.csv`** — cleaned CSV (681 courses)
- **`raw/calpads-course-codes.csv`** — original raw export

See [Credential Requirements by Course](credential-requirements.md) for a structured breakdown, and the raw CSV for the full list.

---

## How to Determine If a Teacher Is Properly Credentialed

1. Find the course's **CALPADS course code** (from the school's master schedule / CALPADS submission).
2. Look up that code in `data/calpads-course-codes.csv`.
3. Read the **"Credentials Authorizing Course"** column.
4. Compare against the teacher's actual credential(s) and their authorization statements.

**Example:** Course code `7100` (Introduction to Agriculture and Natural Resources) is fully authorized by:
- **CTE: Agriculture and Natural Resources** credential, OR
- **Single Subject: Agriculture** credential (at employing agency's discretion).

A teacher holding only a Single Subject: Mathematics credential would **not** be properly credentialed for this course.

---

## Source

- CTC "Appropriate Credentials for CALPADS Course Codes": https://www.ctc.ca.gov/employers/calsaas/calpads-course-codes/
- Raw data: `raw/calpads-course-codes.csv`, `raw/calpads-course-codes-data.txt`

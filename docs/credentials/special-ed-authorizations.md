# Special Education Authorization Matrix

This document details which **disability categories** each special education authorization covers, based on the CTC **Authorization Sort Table** (the "Assignments Authorized by Special Education Authorizations" table).

> **Source:** CTC Authorization Sort Table — https://www.ctc.ca.gov/employers/assignment-resources/assignment-monitoring/credential-authorizations/ (raw: `raw/auth-sort-data.txt`, `raw/auth-sort.html`). Downloaded 2026-08-28.

**Legend:** ✓ = Authorizes service for the disability category; X = Does not authorize service in the identified disability area. \* = These authorizations may only be added to a base special education teaching credential as an Added Authorization (AA).

---

## Modern Support-Need Authorizations

> **Source:** `raw/auth-sort-data.txt` (modern support-need rows).

| Credential / Authorization | Code | Grade Level | Student Support Level | Autism | Emotional Disturbance | Intellectual Disability | Established Medical Disability | Multiple Disabilities | Orthopedic Impairments | Other Health Impairment | Specific Learning Disability | Traumatic Brain Injury | Deafness/Hard of Hearing | Deafblindness | Visual Impairments | Resource Specialist |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Mild to Moderate Support Needs** | `R3MN` | TK–12 (up to age 22), Adult Ed | Mild to Moderate only | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | X | X | ✓ | X | ✓ |
| **Extensive Support Needs** | `R3EN` | TK–12 (up to age 22), Adult Ed | Extensive only | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | X | ✓ | X | ✓ | X |
| **Deaf and Hard of Hearing** | `R3HD` | Birth–age 22, Adult Ed | All | X | X | X | X | X | X | X | X | ✓ | ✓ | X | ✓ | X |
| **Early Childhood Special Education** | `R3ER` | Birth–K | All | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | X | X | ✓ | X |
| **Visual Impairments** | `R3VB` | Birth–age 22, Adult Ed | All | X | X | X | X | X | X | X | X | X | ✓ | ✓ | ✓ | X |

---

## Bridge Authorizations

> **Source:** `raw/auth-sort-data.txt` (bridge authorization rows).

| Bridge Authorization | Code | Grade Level | Covers | Notes |
|----------------------|------|-------------|--------|-------|
| **Education Specialist Bridge – Mild to Moderate Support Needs** | `R3BM` | TK–12 (up to age 22), Adult Ed | Mild to Moderate only, for disabilities unauthorized by R3MM | ✓✓✓✓✓✓✓ (all except deaf/hard of hearing, deafblind, VI) |
| **Education Specialist Bridge – Extensive Support Needs** | `R3BE` | TK–12 (up to age 22), Adult Ed | Extensive only, for disabilities unauthorized by R3MS | ✓✓✓✓✓✓✓ X ✓ X ✓ X |
| **Education Specialist Bridge – Early Childhood** | `R3BC` | Birth–K | All | ✓✓✓✓✓✓✓✓✓ X X ✓ X |

---

## Legacy Support-Need Authorizations

> **Source:** `raw/auth-sort-data.txt` (legacy support-need rows).

| Credential | Code | Grade Level | Student Support Level | Autism | Emotional Disturbance | Intellectual Disability | Established Medical Disability | Multiple Disabilities | Orthopedic Impairments | Other Health Impairment | Specific Learning Disability | Traumatic Brain Injury | Deafness/Hard of Hearing | Deafblindness | Visual Impairments | Resource Specialist |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Mild/Moderate** | `R3MM` | TK–12 to Age 22 | All | X | ✓ | ✓ (Mild/Moderate only) | X | ✓ | X | ✓ | ✓ | X | X | X | ✓ | X |
| **Moderate/Severe** | `R3MS` | TK–12 to Age 22 | All | ✓ | ✓ | ✓ (Moderate/Severe only) | X | ✓ | ✓ | X | X | X | X | ✓ | X | ✓ |
| **Deaf and Hard of Hearing** | `R3DH` | Birth–age 22 | All | X | X | X | X | X | X | X | X | ✓ | ✓ | X | ✓ | X |
| **Physical & Health Impairment** | `R3PI` | Birth–age 22 | All | X | X | ✓ | ✓ | ✓ | ✓ | ✓ | X | ✓ | X | X | X | ✓ |
| **Visual Impairment** | `R3VI` | Birth–age 22 | All | X | X | X | X | X | X | X | X | X | ✓ | ✓ | ✓ | X |
| **Early Childhood Special Education** | `R3EC` | Birth–Pre-K | All | ✓ | ✓ | ✓ | ✓ | ✓ | X | ✓ | ✓ | ✓ | X | X | ✓ | X |
| **Language & Academic Development** | `R3LD` | Pre-K–age 22 | All | X | X | X | X | X | X | X | X | X | X | X | ✓ | X |

---

## Added Authorizations (Disability-Specific)

> **Source:** `raw/auth-sort-data.txt` (added authorization rows).

| Added Authorization | Code | Grade Level | Covers |
|---------------------|------|-------------|--------|
| **Autism Spectrum Disorders** | `AAAS` | See base credential | Autism only |
| **Deaf-Blind** | `AADB` | See base credential | Deaf-blind only |
| **Emotional Disturbance** | `AAED` | See base credential | Emotional disturbance only |
| **Orthopedic Impairment** | `AAOI` | See base credential | Orthopedic impairment only |
| **Other Health Impairment** | `AAOH` | See base credential | Other health impairment only |
| **Traumatic Brain Injury** | `AATB` | See base credential | Traumatic brain injury only |
| **Early Childhood** | `ECSE` | Birth–Pre-K | Early childhood |
| **Resource Specialist** | `RSAA` | See base credential | Resource specialist service |
| **Adapted Physical Education** | `APEA` | See base credential | Adapted PE |

---

## Important Notes

> **Source:** `raw/auth-sort-data.txt` (notes/legend); CTC authorization statements for Education Specialist credentials.

1. **Mild/Moderate (R3MM)** is limited to **Mild/Moderate Intellectual Disabilities**; **Moderate/Severe (R3MS)** is limited to **Moderate/Severe Intellectual Disabilities**.
2. **Language and Academic Development (LAD)** authorization allows services across disability areas, limited to students identified with academic communication and language needs (language development, school readiness, social skills, literacy development).
3. **Resource Specialist** may serve as a resource specialist within the grade levels authorized on the document.
4. **Visual Impairment / Deaf and Hard of Hearing** authorizations may teach VI or DHH students who also have autism, but **cannot** serve students with the Autism disability area alone.
5. Added authorizations (AA) marked with \* may only be added to a **base special education teaching credential**.

---

## Source

This matrix is derived from the CTC **Authorization Sort Table** (`raw/auth-sort-data.txt`), which is the official "Assignments Authorized by Special Education Authorizations" reference.

- CTC Authorization Sort Table: https://www.ctc.ca.gov/employers/assignment-resources/assignment-monitoring/credential-authorizations/
- Raw data: `raw/auth-sort-data.txt`, `raw/auth-sort.html`
- Related: CTC Credential Type and Authorization Statements — https://www.ctc.ca.gov/employers/tools-and-resources/credential-type-and-authorization-statements/

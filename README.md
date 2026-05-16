# 🏥 BarangayHealth — Community Health Monitoring System

<div align="center">

![SDG Goal 3](https://img.shields.io/badge/UN%20SDG-Goal%203%3A%20Good%20Health-3A9D23?style=for-the-badge&logo=united-nations&logoColor=white)
![Status](https://img.shields.io/badge/Status-Final%20Submission-1B4F72?style=for-the-badge)
![Course](https://img.shields.io/badge/Course-PC11%20SAD-2E86C1?style=for-the-badge)
![Methodology](https://img.shields.io/badge/Methodology-SDLC%20%7C%20Waterfall-orange?style=for-the-badge)
![Notation](https://img.shields.io/badge/DFD-Gane--Sarson-blueviolet?style=for-the-badge)
![ERD](https://img.shields.io/badge/ERD-Crow's%20Foot%20%7C%203NF-green?style=for-the-badge)

</div>

---

## 📋 Problem Statement

Barangay Health Centers (BHCs) across the Philippines rely heavily on **paper-based record systems**, leading to:

- ❌ Missed immunization schedules due to no reminder system
- ❌ Lost or incomplete patient records
- ❌ Inability to generate health reports without manual tallying
- ❌ Untracked prenatal consultations for at-risk mothers
- ❌ No way for residents to access their own health information

**BarangayHealth** is a web-based Community Health Monitoring System that digitizes and streamlines the clinical workflow of barangay health centers — directly addressing **UN SDG Goal 3: Good Health and Well-Being**, specifically **Target 3.8** (universal health coverage and access to quality healthcare services).

---

## 📖 Project Description

**BarangayHealth** is a full-stack web application designed for barangay-level healthcare management in the Philippines. The system provides:

| Module | Description |
|--------|-------------|
| 👤 User Authentication & RBAC | Role-based access for Admin, BHW, and Resident |
| 🗂️ Resident Profile Management | Centralized digital health records for all constituents |
| 💉 Immunization Tracking | Automated scheduling with next-dose auto-computation |
| 🤰 Prenatal Care Monitoring | Maternal health visit records and follow-up tracking |
| 🩺 Consultation Records | General health consultation logging per resident |
| 📊 Report Generation Engine | Monthly PDF/CSV health summary for administrators |
| 🔔 Notification Service | In-app appointment reminders for residents |

### Architecture Justification

The system follows a **3-Tier MVC Architecture**:
- **Presentation**: React.js + Tailwind CSS (mobile-responsive)
- **Application**: Node.js + Express.js REST API (JWT authentication, bcrypt)
- **Data**: MySQL 8.0 + Sequelize ORM (3NF normalized schema)

This architecture was chosen to enforce **separation of concerns**, allow **independent module testing**, and support future scalability to multiple barangays.

---

## 🎯 SDG Alignment

| SDG Goal | Target | System Contribution |
|----------|--------|---------------------|
| **Goal 3: Good Health & Well-Being** | Target 3.8 — Universal Health Coverage | Ensures all residents have accessible, organized health records |
| **Goal 3: Good Health & Well-Being** | Target 3.b — Health Technologies | Leverages digital technology for community health delivery |

---

## 👤 Contributors

| Name | Role | Assigned Module |
|------|------|----------------|
| Ira Gabrielle Rivera | Solo Developer / System Analyst | All modules — SRS, SDAD, DFD, ERD, Use Cases, Wireframes |

> **Note:** This is a solo submission. All commits, documentation, and models are authored by the student above.

---

## 📁 Repository Structure

```
[SOLO_SDG3_SAD]
├── DOCUMENTATION/
│   ├── 01_SRS_Final.pdf          ← Software Requirements Specification
│   ├── 02_SDAD_Final.pdf         ← Software Design & Analysis Document
│   └── INTERVIEWS/
│       └── interview_notes.md    ← Raw elicitation notes
├── MODELS/
│   ├── DFD/
│   │   ├── dfd_context.png       ← Level -1 Context Diagram
│   │   └── dfd_level0.png        ← Level-0 Major Processes
│   ├── ERD/
│   │   └── erd_crowsfoot.png     ← Logical ERD (Crow's Foot, 3NF)
│   └── USE_CASES/
│       ├── use_case_diagram.png  ← UML 2.5 Use Case Diagram
│       └── uc_narratives.md      ← Detailed Use Case Narratives
├── PROTOTYPE/
│   └── wireframes/               ← High-fidelity UI mockups (WF-01 to WF-07)
└── README.md                     ← This file
```

---

## 🔧 Methodology

```
Requirements Elicitation → SRS Drafting → Use Case Modeling
        ↓
   DFD Modeling (Gane-Sarson) → ERD Design (Crow's Foot, 3NF)
        ↓
   TELOS Feasibility Analysis → 3-Tier Architecture Design
        ↓
   UI/UX Wireframing → Requirements Traceability Matrix
        ↓
   Final Documentation (SRS + SDAD) → GitHub Submission
```

**SDLC Model Used:** Waterfall (structured, documentation-first — appropriate for a well-defined healthcare domain with stable requirements)

---

## 📐 Modeling Standards

| Model | Notation Standard |
|-------|------------------|
| Data Flow Diagrams | Gane-Sarson DFD Notation |
| Entity-Relationship Diagram | Crow's Foot (Normalized to 3NF) |
| Use Case Diagram | UML 2.5 Standard |
| Requirements | MoSCoW Prioritization with "Shall" syntax |

---

## 📦 Documents

| Document | Description | Link |
|----------|-------------|------|
| 📄 SRS Final | Software Requirements Specification | [`DOCUMENTATION/01_SRS_Final.pdf`](DOCUMENTATION/01_SRS_Final.pdf) |
| 📄 SDAD Final | Software Design & Analysis Document | [`DOCUMENTATION/02_SDAD_Final.pdf`](DOCUMENTATION/02_SDAD_Final.pdf) |

---

## 🏫 Academic Information

| Field | Details |
|-------|---------|
| **Course Code** | PC11 — System Analysis and Design |
| **Program** | Bachelor of Science in Information Technology (BSIT) |
| **Year Level** | 2nd Year |
| **Semester** | 2nd Semester, AY 2025–2026 |
| **Submission Date** | May 16, 2026 |
| **Defense Date** | May 18–20, 2026 |

---

## ⚠️ Academic Integrity Notice

All analysis, design documentation, models, and diagrams in this repository represent original work by the student contributor. Any referenced frameworks, SDG materials, or cited sources are properly attributed within the documents.

---

<div align="center">

**BarangayHealth** | PC11 Final Project | AY 2025–2026
*"Digitizing community healthcare, one barangay at a time."*

</div>

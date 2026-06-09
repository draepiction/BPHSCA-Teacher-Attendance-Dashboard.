# BPHSCA Attendance Dashboard

A lightweight, responsive, single-file administrative workspace designed to manage, log, and track course schedule progress and multi-layered attendance metrics for **G12 Kumintang**. 

This system operates entirely on the client side with absolute transparency, storing state details directly inside your local browser cache to preserve your data records safely across session refreshes.

---

## Core Features & Architecture

*   **11-Week Multi-View Selector:** Effortlessly hop between unique tracking matrices for individual academic weeks, or view consolidated, aggregate totals for the whole trimester at a glance.
*   **Dual-Layer Student Profile System:** Features structural tracking for both full-day school absences ($\varnothing$) and granular, fair tracking for partial late arrivals ($\$$).
*   **Granular Course Tracking:** Individually cycle each class slot state between *Attended*, *Late*, or *Absent*, with dynamic visual cross-outs to easily read schedule progression.
*   **Context Documentation:** Dynamically renders contextual input reason-boxes only when an exception status (*Late* or *Absent*) is selected, allowing for clean record-keeping.
*   **Localized Persistence Engine:** Synchronizes configuration states directly to `localStorage` without external database weight or tracking cookies.
*   **Data Safety Controls:** Features native backup tools to export your tracking data as a clean `.json` payload or import configuration backups into another device or workspace safely.

---

## Technical Index & Layout Conventions

### Interface & Status Glossary

| Element | Status Code / Designation | Operational Description |
| :--- | :--- | :--- |
| **Att** | Attended | Confirms absolute presence and completion of the class session. |
| **Late** | Late Arrival | Identifies partial attendance; prompts for context reason text. |
| **Abs** | Absent | Identifies total class session non-attendance; forces context reason text. |
| **◷** | Day Tardy Flag | Marks the entire calendar date column with warning accents for late arrivals. |
| **⦸** | Day Exclusion Mute | Completely isolates and mutes an entire day column if the student is entirely absent. |

### Subject Nomenclature Index

*   **HSA:** Housekeeping and Sanitation Act
*   **Phil.:** Introduction to the Philosophy of the Human Person
*   **UCSP:** Understanding Culture, Society, and Politics
*   **EAPP:** English for Academic and Professional Purposes
*   **A&E:** Apprenticeship & Exploration (Mr. Divino)
*   **MIL:** Media and Information Literacy
*   **PEH 3:** Physical Education and Health 3
*   **HGP:** Homeroom Guidance Program

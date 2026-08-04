# NERC Standards Map (RC Exam Testable)

**Verified 2026-08-03** against:

- *Exam Resource Materials for NERC System Operator Certification Examinations*,
  January 24, 2025 (current revision)
- *Certification Examination Content Outline — Reliability Coordinator Operator (RC)*,
  effective June 1, 2023 (current; last revised 05/08/2023)
- *System Operator Certification Program Manual* V4.2, February 2025
- NERC ALIGN one-stop-shop standards register (status and effective dates)

Every version suffix and effective date below was checked against NERC's enforcement
register on 2026-08-03. Standards marked **FUTURE** are approved but not yet enforceable.

---

## Exam Format (confirmed current)

| Parameter | Value |
|---|---|
| Total questions | 140 |
| Scored questions | 120 |
| Experimental (unscored) | 20 |
| Cut score (RC) | **92 / 120** (effective June 1, 2020) |
| Examination time | 3 hours |
| Computer-based tutorial | 15 minutes (before the exam clock) |
| Total seat time | 3.25 hours |

Cut scores for other credentials: TOP 76/100, BI&T 92/120, BI 76/100.
Restroom breaks do **not** stop the examination clock.

### Question cognitive levels

NERC writes every question to one of three levels. Expect roughly balanced coverage:

- **Recall** — recognition of isolated information found directly in a source.
- **Application** — interpretation of data; applying knowledge, facts, and rules to solve
  a problem.
- **Analysis** — integration of multiple concepts; judging the effectiveness or
  appropriateness of a course of action.

---

## Approved References (from the January 2025 Exam Resource Materials)

The exam is not written solely from NERC standards. The approved reference list is:

**NERC Reliability Standards** — primary interest to the **NERC Glossary of Terms** and
the **BAL, COM, EOP, FAC, INT, IRO, PRC, TOP, and VAR** standards.
(Note: PER standards are *not* on the primary-interest list even though PER-003 is the
standard that requires your certification.)

**Textbooks and technical references:**

| Reference | Focus |
|---|---|
| *Power System Operation*, 3rd Ed. — Miller & Malinowski | Chapters 1–3, 5–6, 10–12 |
| *EPRI Power System Dynamics Tutorial* (1016042, July 2009) | Glossary, chapters 2–9 and 11 |
| *EPRI Power System Dynamics Tutorial – Supplement* (July 2009) | Supplement to the above |
| *Power System SCADA and Smart Grids*, 1st Ed. — Thomas & McDonald | SCADA and EMS sections |
| *Practical Power System Operation*, 1st Ed. — Vaahedi | Chapters 2–8, 10, 12 |
| *Electricity Generation Baseline Report* (NREL, Jan 2017) | Chapters 5–13 |
| *Active Power Controls from Wind Power: Bridging the Gaps* (Jan 2014) | Chapters 3–4 |

The EPRI tutorial and both DOE/NREL reports are free downloads. Domain 2.c "Electrical
Fundamentals" and 1.h "Energy Sources" draw heavily on these rather than on standards.

---

## Domain 1 — Resource and Demand Balancing (26 scored questions)

| Standard | Eff. | Name | Key Focus |
|---|---|---|---|
| BAL-001-2 | 2016-07-01 | Real Power Balancing Control Performance | CPS1, BAAL, Reporting ACE |
| BAL-002-3 | 2019-04-01 | Disturbance Control Standard — Contingency Reserve | 15-min recovery, 90-min restoration, MSSC |
| BAL-003-2 | 2020-12-01 | Frequency Response and Frequency Bias Setting | FRO, bias settings |
| BAL-005-1 | 2019-01-01 | Balancing Authority Control | Reporting ACE data quality |
| INT-006-5 | 2021-04-01 | Evaluation of Interchange Transactions | Reliability assessment of interchange |
| INT-009-3 | 2021-04-01 | Implementation of Interchange | Implementing Confirmed Interchange |
| IRO-001-4 | 2017-04-01 | Reliability Coordination — Responsibilities | RC authority, Operating Instructions |

**BAL-005-1 testable thresholds:**
- R1 — design scan rate **no more than 6 seconds** for data used to calculate Reporting ACE
- R2 — BA unable to calculate Reporting ACE for **more than 30 consecutive minutes** must
  notify its RC **within 45 minutes** of the beginning of the inability
- R3 — frequency metering available **≥ 99.95%** each calendar year, accuracy **0.001 Hz**

**BAL-002-3 clocks:** Contingency Event Recovery Period = **15 minutes**. Contingency
Reserve Restoration Period = **not exceeding 90 minutes** after that. A Balancing
Contingency Event before the end of a Restoration Period **resets** the beginning of the
Recovery Period.

### Subtopics (question counts from the Content Outline)
- 1.a Interchange Scheduling and Coordination (3)
- 1.b Reserves — Spinning and Non-Spinning (4)
- 1.c Automatic Generation Control (AGC) (3)
- 1.d Area Control Error (ACE) (4)
- 1.e Frequency (4)
- 1.f Load Forecasting (3)
- 1.g Generation Equipment (3)
- 1.h Energy Sources — hydroelectric, solar, thermal (2)

---

## Domain 2 — Transmission (27 scored questions)

| Standard | Eff. | Name | Key Focus |
|---|---|---|---|
| FAC-001-4 | 2024-01-01 | Facility Interconnection Requirements | Requirements for connecting to BES |
| FAC-002-4 | 2024-01-01 | Facility Interconnection Studies | Impact studies for interconnections |
| FAC-003-5 | 2024-04-01 | Transmission Vegetation Management | Vegetation-related outage prevention |
| FAC-008-5 | 2021-10-01 | Facility Ratings | Facility Rating methodology |
| **FAC-011-4** | 2024-04-01 | **SOL Methodology for the Operations Horizon** | How SOLs are established |
| FAC-014-3 | 2024-04-01 | Establish and Communicate System Operating Limits | SOL communication |
| TOP-001-6 | 2024-04-01 | Transmission Operations | TOP obligations, 30-min RTA |
| TOP-002-5 | 2025-10-01 | Operations Planning | Next-day and current-day planning |
| TOP-003-6.1 | 2025-07-01 | TOP and BA Data and Information Specification | Data specifications |
| TOP-010-1(i) | 2018-04-01 | Real-time Reliability Monitoring and Analysis Capabilities | TOP analysis tool quality |
| PRC-004-6 | 2021-04-01 | Protection System Misoperation Identification and Correction | Misoperation analysis |
| PRC-005-6 | 2016-01-01 | Protection System, Automatic Reclosing, and Sudden Pressure Relaying Maintenance | Maintenance and testing |
| PRC-006-5 | 2021-04-01 | Automatic Underfrequency Load Shedding | UFLS program |
| PRC-010-2 | 2017-04-02 | Undervoltage Load Shedding | UVLS program |
| PRC-012-2 | 2021-01-01 | Remedial Action Schemes | RAS design and review |
| PRC-019-2 | 2016-07-01 | Coordination of Generating Unit Capabilities, Voltage Regulating Controls, and Protection | Generator voltage/protection coordination |
| PRC-023-6 | 2024-04-01 | Transmission Relay Loadability | Relay settings vs. ratings |
| PRC-024-3 | 2022-10-01 | Frequency and Voltage Protection Settings for Generators | Generator ride-through |
| PRC-025-2 | 2018-07-01 | Generator Relay Loadability | Generator relay settings |
| PRC-026-2 | 2024-04-01 | Relay Performance During Stable Power Swings | Relay behavior during swings |
| PRC-027-1 | 2021-04-01 | Coordination of Protection Systems for Performance During Faults | Protection coordination |
| PRC-002-5 | 2025-04-01 | Disturbance Monitoring and Reporting Requirements | DME, SER, DDR |
| PRC-028-1 | 2025-04-01 | Disturbance Monitoring and Reporting Requirements for IBRs | IBR disturbance monitoring |
| VAR-001-5 | 2019-01-01 | Voltage and Reactive Control | Voltage schedules |
| VAR-002-4.1 | 2017-09-26 | Generator Operation for Maintaining Network Voltage Schedules | Generator AVR/voltage |

**FAC-011-4 and FAC-014-3 both took effect 2024-04-01** as a pair (Project 2015-09). They
rewrote how SOLs are established and communicated, and they are why the SOL and System
Voltage Limit glossary definitions changed on the same date. If your study material
predates April 2024, its SOL methodology content is stale.

**TOP-001-6 R13:** the TOP shall ensure a Real-time Assessment is performed **at least
once every 30 minutes**. VRF High.

### Subtopics
- 2.a Protection and Control (4)
- 2.b Voltage and Reactive (5)
- 2.c Electrical Fundamentals (4)
- 2.d Reconfiguration and Switching (4)
- 2.e Operating Limits (5)
- 2.f Transmission Equipment (5)

---

## Domain 3 — Emergency Preparedness (12 scored questions)

| Standard | Eff. | Name | Key Focus |
|---|---|---|---|
| EOP-004-4 | 2019-04-01 | Event Reporting | Reportable BES events |
| EOP-005-3 | 2019-04-01 | System Restoration from Blackstart Resources | Blackstart plans |
| EOP-006-3 | 2019-04-01 | System Restoration Coordination | RC restoration coordination |
| EOP-008-2 | 2019-04-01 | Loss of Control Center Functionality | Backup control center |
| **EOP-010-1** | 2015-04-01 | **Geomagnetic Disturbance Operations** | GMD operating procedures |
| EOP-011-4 | 2024-10-01 | **Emergency Operations** | Emergency plans, EEA levels |
| **EOP-012-3** | 2025-10-01 | **Extreme Cold Weather Preparedness and Operations** | Cold weather readiness |
| IRO-017-1 | 2017-04-01 | Outage Coordination | Planned outage review |

**EOP-011-4 renamed the standard** from "Emergency Preparedness and Operations" to
**"Emergency Operations"** effective 2024-10-01, and cold weather content split out into
the EOP-012 series. EEA levels live in **EOP-011-4 Attachment 1**.

**EOP-010-1** is the GMD operating standard and maps directly onto Content Outline
subtopic 3.b (Weather, Natural Disasters, and Geomagnetic Disturbances). It is easy to
miss because GMD is not a defined Glossary term.

### Subtopics
- 3.a Same-Day and Next-Day Planning (4)
- 3.b Weather, Natural Disasters, and Geomagnetic Disturbances (4)
- 3.c Anticipated Capacity Deficiency (4)

---

## Domain 4 — Emergency Response (18 scored questions)

| Standard | Eff. | Name | Key Focus |
|---|---|---|---|
| EOP-011-4 | 2024-10-01 | Emergency Operations | EEA levels, emergency procedures |
| EOP-005-3 | 2019-04-01 | System Restoration from Blackstart Resources | Restoration execution |
| EOP-006-3 | 2019-04-01 | System Restoration Coordination | RC role in restoration |
| EOP-008-2 | 2019-04-01 | Loss of Control Center Functionality | Loss of control center response |
| IRO-001-4 | 2017-04-01 | Reliability Coordination — Responsibilities | RC authority in emergencies |
| IRO-014-3 | 2017-04-01 | Coordination Among Reliability Coordinators | Inter-RC coordination |
| IRO-018-1(i) | 2018-04-01 | RC Real-time Reliability Monitoring and Analysis Capabilities | Response to loss of tools |
| COM-002-4 | 2016-07-01 | Operating Personnel Communications Protocols | Emergency communications |

**IRO-001-4 requirement structure** (all VRF High):
- R1 — the RC shall act to address reliability of its RC Area via **direct actions or by
  issuing Operating Instructions**
- R2 — TOP, BA, GOP, and DP shall **comply** with the RC's Operating Instructions **unless**
  compliance cannot be physically implemented **or** would violate safety, equipment,
  regulatory, or statutory requirements
- R3 — the entity shall **inform its RC** of its inability to perform the Operating
  Instruction

### Subtopics
- 4.a System Restoration (5)
- 4.b Response to System Disturbances (4)
- 4.c Response to Capacity Emergencies (4)
- 4.d Response to Loss of Control Center (2)
- 4.e Response to Loss of Analysis and Monitoring Tools (3)

---

## Domain 5 — Contingency Analysis and Reliability (25 scored questions)

| Standard | Eff. | Name | Key Focus |
|---|---|---|---|
| IRO-002-7 | 2021-04-01 | Reliability Coordination — Monitoring and Analysis | RC tools and monitoring |
| IRO-006-5 | 2011-07-01 | Reliability Coordination — Transmission Loading Relief | TLR framework |
| IRO-006-EAST-2 | 2016-04-01 | TLR Procedure for the Eastern Interconnection | Eastern TLR |
| IRO-006-WECC-3 | 2019-10-01 | Qualified Path Unscheduled Flow Relief | WECC USF relief |
| IRO-008-3 | 2024-04-01 | RC Operational Analyses and Real-time Assessments | Next-day and real-time analysis |
| IRO-009-2 | 2016-01-01 | RC Actions to Operate Within IROLs | IROL mitigation within Tv |
| IRO-010-5 | 2025-07-01 | RC Data and Information Specification and Collection | What data the RC can request |
| IRO-014-3 | 2017-04-01 | Coordination Among Reliability Coordinators | Inter-RC coordination |
| IRO-017-1 | 2017-04-01 | Outage Coordination | Outage assessment |
| IRO-018-1(i) | 2018-04-01 | RC Real-time Reliability Monitoring and Analysis Capabilities | Data quality, alarm monitoring |
| FAC-011-4 | 2024-04-01 | SOL Methodology for the Operations Horizon | SOL/IROL establishment |
| FAC-014-3 | 2024-04-01 | Establish and Communicate SOLs | SOL communication |
| TOP-010-1(i) | 2018-04-01 | Real-time Reliability Monitoring and Analysis Capabilities | TOP counterpart to IRO-018 |

**IRO-008-3 R4:** the RC shall ensure a Real-time Assessment is performed **at least once
every 30 minutes**. VRF High. This mirrors TOP-001-6 R13 for the TOP.

**IRO-009-2 requirement structure:**
- R1 — develop Operating Processes/Procedures/Plans that can be implemented **in time to
  prevent** the identified IROL exceedance
- R2 — initiate those processes to prevent an IROL exceedance
- R3 — act or direct others to act so the magnitude and duration of an IROL exceedance is
  mitigated **within the IROL's Tv**
- R4 — where RCs differ on an IROL or its Tv, **operate to the most limiting IROL and Tv**

### Subtopics
- 5.a Contingency Analysis (5)
- 5.b Network Analysis Tools — e.g., State Estimators (5)
- 5.c Response to Results of Contingency Analysis (5)
- 5.d System Operating Limits (SOL) (5)
- 5.e Interconnection Reliability Operating Limits (IROL) (5)

---

## Domain 6 — Communications and Data (12 scored questions)

| Standard | Eff. | Name | Key Focus |
|---|---|---|---|
| COM-001-3 | 2017-10-01 | Communications | Telecom infrastructure, Alternative Interpersonal Communication |
| COM-002-4 | 2016-07-01 | Operating Personnel Communications Protocols | Three-part communication |
| IRO-002-7 | 2021-04-01 | Reliability Coordination — Monitoring and Analysis | Data and monitoring tools |
| IRO-010-5 | 2025-07-01 | RC Data and Information Specification and Collection | RC data specification |
| IRO-018-1(i) | 2018-04-01 | RC Real-time Monitoring and Analysis Capabilities | Data quality and alarms |
| TOP-003-6.1 | 2025-07-01 | TOP and BA Data and Information Specification | TOP/BA data specification |
| EOP-004-4 | 2019-04-01 | Event Reporting | Reporting obligations |

**COM-002-4 requirement structure — this is the highest-yield structure in the domain:**

| Req | Who | What | VRF |
|---|---|---|---|
| R1 | BA, RC, TOP | Develop documented communications protocols (English unless agreed; issuer/receiver actions; burst instructions; time identification; Element nomenclature) | Low |
| R2 | BA, RC, TOP | Initial training before issuing an Operating Instruction | Low |
| R3 | DP, GOP | Initial training before receiving an oral two-party Operating Instruction | Low |
| R4 | BA, RC, TOP | **At least once every 12 calendar months**: assess *adherence* (with feedback and corrective action) and assess *effectiveness* of the protocols | Medium |
| R5 | BA, RC, TOP | Issuer three-part actions **during an Emergency** | **High** |
| R6 | BA, DP, GOP, TOP | Receiver three-part actions **during an Emergency** | **High** |
| R7 | BA, RC, TOP | Burst Operating Instruction during an Emergency: confirm or verify receipt | **High** |

Three-part specifics:
- The receiver repeats the Operating Instruction **"not necessarily verbatim"** and
  receives confirmation, **or** requests the issuer reissue it.
- The issuer confirms if repeated information is correct; reissues if incorrect or if
  requested; or takes an **alternative action** if no response is received or the
  instruction was not understood.
- For a **single-party to multiple-party burst** Operating Instruction, the issuer need
  only confirm or verify receipt by **at least one receiver** — burst instructions are
  explicitly *excluded* from the R5/R6 two-party three-part requirements.

### Subtopics
- 6.a Reporting Requirements (3)
- 6.b Communication Methods — e.g., Three-Part Communication, RCIS (3)
- 6.c Data Validity and Verification (4)
- 6.d Telemetry and Communications Equipment (2)

---

## Changing Soon — Know the Dates

| Standard | Status | Date | Note |
|---|---|---|---|
| PRC-024-4 | FUTURE | 2026-10-01 | Replaces PRC-024-3; retitled "…for Synchronous Generators" |
| PRC-029-1 | FUTURE | 2026-10-01 | Frequency and Voltage Ride-through Requirements for IBRs |
| PRC-030-1 | FUTURE | 2026-10-01 | Unexpected Inverter-Based Resource Event Mitigation |
| TOP-003-7 | FUTURE | 2026-10-01 | Replaces TOP-003-6.1 |
| EOP-004-5 | Filed, pending regulatory approval | — | **EOP-004-4 remains enforceable** |
| BAL-007-1.1 | FUTURE | 2027-04-01 | Near-Term Energy Reliability Assessments |
| PRC-008-0, PRC-011-0, PRC-017-1 | Retiring | 2027-03-31 | UFLS/UVLS/RAS maintenance standards |
| IRO-010-6 | FUTURE | 2029-04-01 | Order 901 IBR data specification |
| TOP-003-8 | FUTURE | 2029-04-01 | Order 901 IBR data specification |

The exam tests what is **enforceable on your exam date**. As of 2026-08-03 the
2026-10-01 batch is not yet in force — but if you sit the exam in Q4 2026 or later,
PRC-024-4, PRC-029-1, PRC-030-1, and TOP-003-7 are fair game.

---

## Retired — Do Not Study These

These appear in older study material and make excellent distractors:

| Retired | Replaced by |
|---|---|
| **INT-004** (Dynamic Interchange Transaction Modifications) | Retired; no direct replacement |
| **INT-010** (Interchange Coordination Exemptions) | Retired; no direct replacement |
| **PRC-001** (System Protection Coordination) | PRC-027-1 and PRC-012-2 |
| **IRO-019** | Never existed as a NERC standard |
| **COM-002-3** ("This is a Reliability Directive") | COM-002-4, built on Operating Instruction |
| **PRC-015 / PRC-016** (SPS standards) | PRC-012-2 |

Only **INT-006-5** and **INT-009-3** remain enforceable in the INT family.

---

## PER Standards (context, not primary exam content)

Not on the Exam Resource Materials primary-interest list, but they define your credential:

| Standard | Eff. | Name |
|---|---|---|
| PER-003-2 | 2019-07-01 | Operating Personnel Credentials |
| PER-005-2 | 2016-07-01 | Operations Personnel Training |
| PER-006-1 | 2021-04-01 | Specific Training for Personnel |

**Credential maintenance (SOC Program Manual V4.2):** the RC credential requires **200
CEHs** over the three-year period, including a minimum of **30 CEHs on NERC Reliability
Standards** content/implementation and a minimum of **30 simulation CEHs**. Up to 30 CEHs
may be carried over into the next period.

---

## The 31 RC Task Statements (Content Outline, June 2023)

Exam questions are traceable to these tasks. Several traps key directly off task wording.

1. Adjust flow control devices within the transmission area to maintain reliability.
2. Approve Arranged Interchange from ramping ability perspective.
3. Calculate and monitor area control error.
4. **Curtail Confirmed Interchange that adversely impacts reliability.**
5. Deploy reliability-related services.
6. Determine reliability-related services requirements for balancing generation and load, and transmission reliability.
7. Develop emergency procedures.
8. Develop Interconnection Reliability Operating Limits to protect from instability and Cascading.
9. Develop system limitations such as System Operating Limits and Total Transfer Capabilities, and operate within those limits.
10. Develop system restoration plans.
11. Direct and coordinate system restoration.
12. Direct implementation of emergency procedures including load shedding.
13. Direct revisions to generation maintenance plans as permitted by agreements.
14. Direct revisions to transmission maintenance plans as permitted by agreements.
15. Formulate an operational plan for reliability evaluation.
16. Identify, communicate, and direct actions if necessary to relieve reliability threats and limit violations.
17. Communicate effectively, accurately, and concisely with other parties (adjacent BA, TOPs, RCs, etc.).
18. Implement Confirmed Interchange.
19. Implement emergency procedures.
20. Implement system restoration plans.
21. Interpret actual and contingency reliability analyses.
22. Monitor and adjust reactive resources to maintain transmission voltage within defined limits.
23. Monitor and deploy transmission assets, protective relaying systems, and Remedial Action Schemes (SPS/RAS).
24. Monitor and report control performance and disturbance recovery.
25. Monitor and update all reliability-related parameters within the reliability area.
26. Monitor and update telemetry of reliability-related parameters within the reliability area.
27. Operate in the Balancing Authority Area to maintain load-interchange-generation balance.
28. Operate within established Interconnection Reliability Operating Limits.
29. Perform actual and contingency reliability analyses.
30. Provide balancing and energy accounting, and administer inadvertent energy paybacks.
31. Review generation commitments, dispatch, and load forecasts.

Note tasks 13 and 14: the RC directs revisions to maintenance plans **as permitted by
agreements** — not unilaterally.

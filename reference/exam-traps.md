# NERC RC Exam Traps

Known misconceptions and common wrong answers. The validator checks claims against these.

**Last verified 2026-08-03** against the NERC Glossary, COM-002-4, IRO-001-4, IRO-008-3,
IRO-009-2, TOP-001-6, BAL-002-3, BAL-005-1, EOP-011-4, and the June 2023 RC Content
Outline. Traps 6–9 were **corrected** in this pass; traps 16–28 are new.

---

## TRAP 1 — RC vs. BA vs. TOP Authority
The RC has directive authority over TOPs and BAs. The BA controls generation/load balance.
The TOP controls local transmission. The RC does NOT operate equipment directly — it acts
via direct actions or by issuing Operating Instructions (IRO-001-4 R1).

## TRAP 2 — SOL vs. IROL
ALL IROLs are SOLs, but NOT all SOLs are IROLs. An IROL specifically risks instability,
uncontrolled separation, or Cascading. An SOL violation may only affect a local area.

## TRAP 3 — IROL Tv
Must be ≤ 30 minutes. The RC must act BEFORE Tv expires. 30 minutes is NOT a grace period.
It is the absolute maximum. Corrective action begins immediately upon identification.

## TRAP 4 — Real Power (MW) vs. Reactive Power (MVAR)
Real power → frequency. Reactive power → voltage. Students confuse which controls which.

## TRAP 5 — Frequency vs. Voltage
Frequency is SYSTEM-WIDE across the entire interconnection. Voltage is LOCAL or regional.

## TRAP 6 — COM-002-4 Three-Part Communication *(CORRECTED 2026-08-03)*
Three-part communication is: (1) issuer issues the Operating Instruction, (2) receiver
repeats it back, (3) issuer confirms or reissues. Three details people get wrong:

- The receiver repeats **"not necessarily verbatim."** Word-for-word repetition is NOT
  required. An answer choice demanding verbatim repetition is wrong.
- The **mandatory** three-part requirement (R5/R6, VRF High) applies to oral two-party,
  person-to-person Operating Instructions **during an Emergency**. Outside an Emergency,
  the obligation is to have and follow documented protocols under R1 (VRF Low).
- **Burst** instructions (single-party to multiple-party, written or oral) are explicitly
  **excluded** from R5/R6. For a burst, the issuer need only confirm or verify receipt by
  **at least one receiver** (R1.4, R7).

Also testable: COM-002-4 R4 requires assessing both **adherence** and **effectiveness** of
the protocols **at least once every 12 calendar months**.

## TRAP 7 — EEA Levels Are NOT Sequential *(CORRECTED 2026-08-03)*
EOP-011-4 Attachment 1 states plainly: **"The Reliability Coordinator may declare whatever
alert level is necessary, and need not proceed through the alerts sequentially."**

An answer choice implying the RC must escalate 1 → 2 → 3 in order is **wrong**. The RC can
declare EEA 3 directly if conditions warrant.

Watch the level boundaries too — the distinguishing test is **Contingency Reserves**:

| Level | Test |
|---|---|
| EEA 1 | All available generation committed; **concerned about sustaining** required Contingency Reserves; non-firm wholesale sales curtailed |
| EEA 2 | Load management in effect; BA is energy deficient; **still able to maintain** minimum Contingency Reserves |
| EEA 3 | Firm Load interruption imminent or in progress; BA **unable to meet** minimum Contingency Reserves |

Load management procedures belong to **EEA 2**, not EEA 1. That is the single most common
EEA error.

## TRAP 8 — ATC Equation *(CORRECTED 2026-08-03)*
```
ATC = TTC - ETC - CBM - TRM + Postbacks + Counterflows
```
CBM and TRM are **separate subtractions**. CBM is NOT bundled inside ETC. ETC includes
retail customer service. Postbacks and counterflows ADD back. An answer that folds CBM
into ETC, or omits either margin, is wrong.

## TRAP 9 — "Reliability Directive" Is a Retired Term *(CORRECTED 2026-08-03)*
This is a genuine trap and older study guides get it wrong.

**"Reliability Directive" is not in the current NERC Glossary and appears nowhere in
COM-002-4.** It was deliberately replaced by **Operating Instruction**. The published
rationale in IRO-001-4 says the change was made because directives "should be mandatory at
**all times**, and not just during emergencies."

Consequences:
- There is **no** requirement to say "This is a Reliability Directive." That came from the
  retired COM-002-3.
- Compliance with the RC's Operating Instruction is mandatory at all times (IRO-001-4 R2),
  not only in emergencies.
- If an answer choice hinges on announcing a Reliability Directive, it is testing whether
  you know the term was retired.

## TRAP 10 — Who Calculates IROLs
The RC calculates IROLs. The TOP/BA cannot — they lack the Wide Area view. The RC's purview
is "broad enough to enable the calculation of IROLs, which may be based on the operating
parameters of transmission systems beyond any Transmission Operator's vision."

## TRAP 11 — Three Types of Transmission Limits
Thermal (Facility Ratings), voltage (System Voltage Limits), and stability (stability
limits). The SOL definition names exactly these three. **The most restrictive determines
the SOL.**

## TRAP 12 — Next-Day vs. Real-Time
The RC must perform BOTH operational planning analyses and Real-time Assessments
(IRO-008-3). Not just real-time.

## TRAP 13 — Who Declares EEA Levels
The RC declares EEA levels, NOT the BA. Per EOP-011-4, an EEA "may be initiated **only by a
Reliability Coordinator**," either at the RC's own request or upon request of an energy
deficient BA. The BA identifies the deficiency; the RC declares the alert.

## TRAP 14 — Interchange Curtailment Authority
The RC can curtail Confirmed Interchange that adversely impacts reliability (Task 4). Know
the state progression: **Arranged → Confirmed → Implemented**. Note the actual definitions:
Arranged Interchange = "the state where a Request for Interchange has been submitted for
approval"; Confirmed Interchange = "the state where no party has denied and all required
parties have approved the Arranged Interchange."

## TRAP 15 — State Estimator vs. RTCA
The State Estimator shows the CURRENT state ("what IS happening now"). Real-Time
Contingency Analysis shows what WOULD happen IF a contingency occurs ("what if"). The State
Estimator feeds the RTCA.

---

## TRAP 16 — The 30-Minute Real-time Assessment
Both the RC (**IRO-008-3 R4**) and the TOP (**TOP-001-6 R13**) must ensure a Real-time
Assessment is performed **at least once every 30 minutes**. Both are VRF High.

Do not confuse this 30 minutes with the IROL Tv 30-minute maximum. They are unrelated
numbers that happen to match — which is exactly why the exam uses them as distractors for
each other.

## TRAP 17 — Two Different Contingency Clocks
- **Contingency Event Recovery Period = 15 minutes** — the window to return Reporting ACE
  to its recovery value after a Reportable Balancing Contingency Event.
- **Contingency Reserve Restoration Period = not exceeding 90 minutes** — begins after the
  Recovery Period ends.

A Balancing Contingency Event occurring before the end of a Restoration Period **resets the
beginning of the Recovery Period**. Students merge these into one number.

## TRAP 18 — Reportable Event Thresholds by Interconnection
A Reportable Balancing Contingency Event is one with MW loss ≤ MSSC and ≥ the **lesser of**
80% of MSSC or the Interconnection floor:

| Interconnection | Floor |
|---|---|
| Eastern | 900 MW |
| Western | 500 MW |
| ERCOT | 800 MW |
| Quebec | 500 MW |

Note Eastern (900) and ERCOT (800) are the odd ones — Western and Quebec are both 500.

## TRAP 19 — Most Limiting IROL Between RCs
**IRO-009-2 R4:** where RCs differ on an IROL or its Tv, the RC shall operate to the **most
limiting** IROL and Tv. Not its own, not an average, not the neighbor's — the most limiting.

## TRAP 20 — Misoperation Is About the *Composite* Protection System
A Misoperation is the failure of a **Composite Protection System** to operate as intended.
Failure of an individual Protection System **component** is NOT a Misoperation as long as
the Composite Protection System performs correctly.

There are **six** categories, paired as During Fault / Other Than Fault: Failure to Trip,
Slow Trip, Unnecessary Trip. **"Out-of-zone trip" is not a NERC Misoperation category.**
Operations caused by personnel during on-site maintenance, testing, inspection,
construction, or commissioning are **not** Misoperations.

## TRAP 21 — BES Inclusion Thresholds
20 MVA and 75 MVA do different jobs:

- Individual generating resource: gross nameplate **> 20 MVA**
- Plant/facility **aggregate**: gross nameplate **> 75 MVA**
- Dispersed power producing resources aggregating **> 75 MVA**
- Local networks are excluded when operated **< 300 kV**
- BES baseline voltage is **100 kV or higher**

Do not swap 20 and 75, and do not apply the individual threshold to a plant aggregate.

## TRAP 22 — Operating Instruction Compliance Has Exactly Two Exceptions
Per **IRO-001-4 R2**, a TOP/BA/GOP/DP must comply with the RC's Operating Instruction
unless it (a) **cannot be physically implemented**, or (b) would **violate safety,
equipment, regulatory, or statutory requirements**. "I disagree with it" and "it is
economically unfavorable" are not exceptions. And per R3, the entity must **inform the RC**
of its inability to perform.

## TRAP 23 — Operating Plan vs. Procedure vs. Process
- **Operating Procedure** — specific steps, for specific positions, followed **in the order
  presented**.
- **Operating Process** — general steps with **options selected based on Real-time
  conditions**.
- **Operating Plan** — the container document; may contain both.

The exam tests whether you know a Process allows operator judgment and a Procedure does not.

## TRAP 24 — ACE vs. Reporting ACE
"ACE" is the general concept. **"Reporting ACE"** is the term used for compliance in
BAL-001, BAL-002, and BAL-005. If a question asks what a standard requires, the answer is
framed as Reporting ACE.

Also: the **Frequency Bias Setting B is a negative number**, and the **IIM term is null**
unless a regional inadvertent-control procedure exists for the Interconnection. IIM is
explicitly **not** used for unilateral paybacks.

## TRAP 25 — BAL-005-1 Data Quality Numbers
- Design scan rate: **no more than 6 seconds**
- Unable to calculate Reporting ACE for **more than 30 consecutive minutes** → notify the
  RC **within 45 minutes** of the beginning of the inability
- Frequency metering: **≥ 99.95%** annual availability, **0.001 Hz** accuracy

The 30/45 pairing is the trap — the trigger is 30 minutes, the notification deadline is 45
minutes from the *start* of the outage, not from the 30-minute mark.

## TRAP 26 — Spinning vs. Supplemental Reserve
The distinguishing word is **synchronized**:
- **Operating Reserve – Spinning:** generation **synchronized** to the system, fully
  available within the Disturbance recovery period.
- **Operating Reserve – Supplemental:** generation synchronized **or capable of being
  synchronized**, fully available within the Disturbance Recovery Period.

Both may also be satisfied by load fully removable within the period. Interruptible load
counts as reserve — a point the NERC sample question makes directly.

## TRAP 27 — What Is NOT a RAS
The RAS definition excludes 14 items. The ones most often mistaken for RAS:
- UFLS and UVLS schemes comprised of **only distributed relays**
- Out-of-step tripping and power swing blocking
- Automatic reclosing schemes
- Automatic sequences that proceed when **manually initiated** by a System Operator
- Generator controls: AGC, AVR, PSS, fast valving, speed governing

Also note **SPS** is no longer an independent term — the Glossary carries "Special
Protection System (Remedial Action Scheme): See 'Remedial Action Scheme'." Prefer RAS.

## TRAP 28 — Generator Operator Now Has Two Categories
Effective **2026-01-01**, the GOP definition split:
- **Category 1 GOP** — operates generating Facilities, supplies energy and Interconnected
  Operations Services (the classic definition).
- **Category 2 GOP** — operates **non-BES Inverter-Based Resources** with aggregate
  nameplate **≥ 20 MVA** connected at **≥ 60 kV** to a common point of connection.

Note the Category 2 numbers (20 MVA, 60 kV) differ from the BES inclusion numbers (20 MVA,
100 kV). The voltage is the discriminator.

## TRAP 29 — Cascading and Adverse Reliability Impact Wording
- **Cascading** spreads "beyond **an area predetermined by studies**" — not "a
  predetermined area."
- **Adverse Reliability Impact** is "frequency-related instability; unplanned tripping of
  load or generation; or uncontrolled separation or cascading outages that affects a
  widespread area of the Interconnection." An answer reading "BES instability or Cascading"
  is the **old** definition.

## TRAP 30 — Retired Standards as Distractors
INT-004, INT-010, PRC-001, PRC-015, and PRC-016 are **retired**. IRO-019 never existed.
Only INT-006-5 and INT-009-3 remain enforceable in the INT family. If a question offers a
retired standard as the source of a requirement, it is wrong by construction.

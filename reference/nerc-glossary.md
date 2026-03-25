# NERC Glossary of Terms (RC Exam Relevant)

This file is GROUND TRUTH for all validation. Update as new terms are researched.

---

## Entities

**Reliability Coordinator (RC):** The entity that is the highest level of authority who is responsible for the Reliable Operation of the Bulk Electric System, has the Wide Area view of the Bulk Electric System, and has the operating tools, processes and procedures, including the authority to prevent or mitigate emergency operating situations in both next-day analysis and real-time operations. The Reliability Coordinator has the purview that is broad enough to enable the calculation of Interconnection Reliability Operating Limits (IROLs), which may be based on the operating parameters of transmission systems beyond any Transmission Operator's vision.

**Balancing Authority (BA):** The responsible entity that integrates resource plans ahead of time, maintains Demand and resource balance within a Balancing Authority Area, and supports Interconnection frequency in real time.

**Transmission Operator (TOP):** The entity responsible for the reliability of its local transmission system, and that operates or directs the operations of the transmission Facilities.

**Generator Operator (GOP):** The entity that operates generating unit(s) and performs the functions of supplying energy and Interconnected Operations Services.

---

## System Limits

**Interconnection Reliability Operating Limit (IROL):** A System Operating Limit that, if violated, could lead to instability, uncontrolled separation, or Cascading outages that adversely impact the reliability of the Bulk Electric System.

**System Operating Limit (SOL):** The value (such as MW, MVAR, amperes, frequency, or volts) that satisfies the most limiting of the prescribed operating criteria for a specified system configuration to ensure operation within acceptable reliability criteria.

**Tv (IROL Tv):** The maximum time that an IROL can be violated before the risk to the interconnection or other Reliability Coordinator Area(s) becomes greater than acceptable. Each IROL's Tv shall be less than or equal to 30 minutes.

**Facility Rating:** The maximum or minimum voltage, current, frequency, or real or reactive power flow through a Facility that does not violate the applicable equipment rating of any equipment comprising the Facility.

**Thermal Rating:** The maximum amount of electrical current that a transmission line or electrical facility can conduct over a specified time period before it sustains permanent damage by overheating or before it violates public safety requirements.

---

## Transfer Capability

**Available Transfer Capability (ATC):** A measure of the transfer capability remaining in the physical transmission network for further commercial activity over and above already committed uses.

**Total Transfer Capability (TTC):** The amount of electric power that can be moved or transferred reliably from one area to another area of the interconnected transmission systems by way of all transmission lines (or paths) between those areas under specified system conditions.

**Transmission Reliability Margin (TRM):** The amount of transmission transfer capability necessary to provide reasonable assurance that the interconnected transmission network will be secure.

**Capacity Benefit Margin (CBM):** The amount of firm transmission transfer capability preserved by the transmission provider for Load-Serving Entities (LSEs) to enable access to generation from interconnected systems to meet generation reliability requirements.

**ATC Equation:** ATC = TTC - TRM - Existing Transmission Commitments (including CBM) + Postbacks + Counterflows

---

## Balancing

**Area Control Error (ACE):** The instantaneous difference between a Balancing Authority's net actual and scheduled interchange taking into account the effects of Frequency Bias, correction for meter error, and Automatic Time Error Correction.

**ACE Equation:** ACE = (NIA - NIS) - 10B(FA - FS) - IME
- NIA = Net Interchange Actual (MW)
- NIS = Net Interchange Scheduled (MW)
- B = Frequency Bias Setting (MW/0.1 Hz, negative number)
- FA = Frequency Actual (Hz)
- FS = Frequency Scheduled (Hz, normally 60.000)
- IME = Interchange Meter Error (MW)

**Frequency Response:** Equipment response as a result of a change in system frequency.

---

## Power Fundamentals

**Real Power:** The component of electric power that performs work, measured in watts (W) or megawatts (MW). Associated with resistive load. Controls system frequency.

**Reactive Power:** The component of electric power that establishes and sustains the electric and magnetic fields of AC equipment, measured in volt-amperes reactive (VAR) or megavolt-amperes reactive (MVAR). Does NOT perform useful work. Maintains system voltage.

**Power Factor:** The ratio of Real Power (MW) to Apparent Power (MVA). Power Factor = MW / MVA.

**Apparent Power:** The product of voltage and current in an AC circuit, measured in MVA. Apparent Power = √(Real Power² + Reactive Power²)

---

## Emergency

**Energy Emergency Alert (EEA):**
- EEA Level 1: All available generation resources are committed, firm load management has been implemented, non-firm wholesale energy purchases have been curtailed.
- EEA Level 2: Load management procedures being implemented. Circumstances may require reducing firm load.
- EEA Level 3: Firm load interruption is imminent or in progress.

**Cascading:** The uncontrolled successive loss of System Elements triggered by an incident at any location. Results in widespread electric service interruption that cannot be restrained from sequentially spreading beyond a predetermined area.

**Adverse Reliability Impact:** The impact of an event that results in Bulk Electric System instability or Cascading.

---

## Communications

**Operating Instruction:** A command by a system operator that requires a change in or maintains a specific state of an Element, Facility, or Interconnected Elements. Not a discussion of general information.

**Reliability Directive:** A communication initiated by an RC, TOP, or BA where action by the recipient is necessary to address an actual or expected Emergency. A Reliability Directive is a subset of Operating Instructions.

---

## Other

**Bulk Electric System (BES):** All Transmission Elements operated at 100 kV or higher and Real Power and Reactive Power resources connected at 100 kV or higher, unless specifically excluded.

**Contingency:** The unexpected failure or outage of a system component.

**N-1 Contingency:** System remains stable and within limits after the loss of any single element.

**N-2 Contingency:** System remains stable and within limits after the loss of any two elements.

**Curtailment:** A reduction in the scheduled capacity or energy delivery.

**Transmission Loading Relief (TLR):** A procedure used in the Eastern Interconnection as a congestion management tool.

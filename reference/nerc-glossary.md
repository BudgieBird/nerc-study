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

**System Operating Limit (SOL):** All Facility Ratings, System Voltage Limits, and stability limits, applicable to specified System configurations, used in Bulk Electric System operations for monitoring and assessing pre- and post-Contingency operating states.

**Tv (IROL Tv):** The maximum time that an IROL can be violated before the risk to the interconnection or other Reliability Coordinator Area(s) becomes greater than acceptable. Each IROL's Tv shall be less than or equal to 30 minutes.

**Facility Rating:** The maximum or minimum voltage, current, frequency, or real or reactive power flow through a Facility that does not violate the applicable equipment rating of any equipment comprising the Facility.

**Thermal Rating:** The maximum amount of electrical current that a transmission line or electrical facility can conduct over a specified time period before it sustains permanent damage by overheating or before it sags to the point that it violates public safety requirements.

---

## Transfer Capability

**Available Transfer Capability (ATC):** A measure of the transfer capability remaining in the physical transmission network for further commercial activity over and above already committed uses.

**Total Transfer Capability (TTC):** The amount of electric power that can be moved or transferred reliably from one area to another area of the interconnected transmission systems by way of all transmission lines (or paths) between those areas under specified system conditions.

**Transmission Reliability Margin (TRM):** The amount of transmission transfer capability necessary to provide reasonable assurance that the interconnected transmission network will be secure.

**Capacity Benefit Margin (CBM):** The amount of firm transmission transfer capability preserved by the transmission provider for Load-Serving Entities (LSEs) to enable access to generation from interconnected systems to meet generation reliability requirements.

**ATC Equation:** ATC = TTC - TRM - Existing Transmission Commitments (including CBM) + Postbacks + Counterflows

---

## Balancing

**Area Control Error (ACE):** The instantaneous difference between a Balancing Authority's net actual and scheduled interchange taking into account the effects of Frequency Bias, correction for meter error, and Inadvertent Interchange Management (IIM).

**ACE Equation:** ACE = (NIA - NIS) - 10B(FA - FS) - IME + IIM
- NIA = Net Interchange Actual (MW)
- NIS = Net Interchange Scheduled (MW)
- B = Frequency Bias Setting (MW/0.1 Hz, negative number)
- FA = Frequency Actual (Hz)
- FS = Frequency Scheduled (Hz, normally 60.000)
- IME = Interchange Meter Error (MW)
- IIM = Inadvertent Interchange Mitigation (MW, replaces legacy Automatic Time Error Correction term)

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

**Operating Instruction:** A command by operating personnel responsible for the Real-time operation of the interconnected Bulk Electric System to change or preserve the state, status, output, or input of an Element of the Bulk Electric System or Facility of the Bulk Electric System. A discussion of general information and of potential options or alternatives to resolve BES operating concerns is not a command and is not considered an Operating Instruction.

**Reliability Directive:** A communication initiated by an RC, TOP, or BA where action by the recipient is necessary to address an actual or expected Emergency. A Reliability Directive is a subset of Operating Instructions.

---

## Other

**Bulk Electric System (BES):** All Transmission Elements operated at 100 kV or higher and Real Power and Reactive Power resources connected at 100 kV or higher, unless specifically excluded.

**Contingency:** The unexpected failure or outage of a system component.

**N-1 Contingency:** System remains stable and within limits after the loss of any single element.

**N-2 Contingency:** System remains stable and within limits after the loss of any two elements.

**Curtailment:** A reduction in the scheduled capacity or energy delivery.

**Transmission Loading Relief (TLR):** A procedure used in the Eastern Interconnection as a congestion management tool.

---

## Protection and Control

**Remedial Action Scheme (RAS):** A scheme designed to detect predetermined System conditions and automatically take corrective actions that may include, but are not limited to, adjusting or tripping generation, tripping load, or reconfiguring a System to maintain System reliability. Also known as Special Protection System (SPS).

**Special Protection System (SPS):** See Remedial Action Scheme (RAS). Legacy term still used on the exam interchangeably with RAS.

**Underfrequency Load Shedding (UFLS):** Automatic tripping of load when system frequency drops below predetermined thresholds. Designed to arrest frequency decline and prevent system collapse. Defined in PRC-006.

**Undervoltage Load Shedding (UVLS):** Automatic tripping of load when voltage drops below predetermined thresholds. Prevents voltage collapse. Defined in PRC-010.

**Protection System:** The collection of protection equipment and communications systems necessary to detect faults and initiate corrective actions to maintain BES reliability. Includes relays, CTs, PTs, communications, and trip circuits.

**Misoperation:** The failure of a Protection System to operate as intended. Includes failure to trip, slow trip, unnecessary trip, and out-of-zone trip. Tracked under PRC-004.

---

## Voltage and Reactive

**Voltage Schedule:** The voltage set point and tolerance band for a specific bus, established by the TOP or RC. Generators must operate within their voltage schedule per VAR-002.

**Automatic Voltage Regulator (AVR):** Equipment on a generator that automatically adjusts field excitation to maintain terminal voltage at the set point. Must be in service per VAR-002 unless exempted.

**Power System Stabilizer (PSS):** Equipment that provides supplementary control signals to the generator's AVR to dampen power oscillations and improve dynamic stability.

**Voltage Collapse:** Progressive and uncontrollable decline in voltage caused by insufficient reactive power support. Can lead to cascading outages.

**Reactive Power Compensation:** Devices that supply or absorb reactive power to maintain voltage: capacitor banks (supply MVAR, raise voltage), reactors (absorb MVAR, lower voltage), SVCs, STATCOMs, synchronous condensers.

---

## Interchange

**Arranged Interchange:** The state of an Interchange Transaction after the Interchange Authority has verified that the transaction is valid and balanced. Precedes Confirmed Interchange.

**Confirmed Interchange:** The state of an Interchange Transaction after all participating BAs have confirmed the arrangement. The RC must evaluate for reliability impact per INT-006.

**Interchange Transaction:** A request to transfer energy across BA boundaries that must be evaluated, confirmed, and implemented through the interchange scheduling process.

**Interchange Authority:** The entity that authorizes implementation of valid and balanced Interchange Schedules between BAs.

**Dynamic Interchange Transaction:** An Interchange Transaction where the MW value is adjusted in real time to follow varying load or generation patterns. May be modified per INT-004.

---

## Analysis Tools

**State Estimator:** A software tool that uses real-time telemetry data to calculate the most likely state of the power system. Produces a solved power flow model of current system conditions. Critical for contingency analysis (IRO-008, IRO-018).

**Contingency Analysis:** The assessment of potential system conditions following the loss of one or more elements (N-1, N-2). Uses the state estimator model to evaluate whether remaining facilities would exceed ratings or limits. RC must perform both next-day and real-time (IRO-008).

**Real-Time Contingency Analysis (RTCA):** Automated, continuous contingency analysis that runs against the current state estimator solution. Identifies potential SOL/IROL violations before they occur.

**Real-Time Assessment:** The evaluation of actual system conditions to determine if SOLs or IROLs are being exceeded and whether the system is in a secure operating state. Required by IRO-008.

---

## Switching and Reconfiguration

**Switching Order:** A documented sequence of switching steps for opening/closing circuit breakers, disconnects, and other devices to achieve a desired system configuration. Must be communicated using three-part communication per COM-002.

**Clearance:** The isolation of equipment from all energy sources to permit safe maintenance. Requires proper tagging procedures and verification.

**Tagging:** The process of applying tags to equipment to indicate it is isolated and not to be operated. Part of the clearance process.

---

## Generation and Energy Sources

**Automatic Generation Control (AGC):** A system that automatically adjusts generator output to maintain ACE at or near zero. Responds to frequency deviations and interchange schedule errors.

**Spinning Reserve:** Unloaded generation that is synchronized to the system and ready to serve additional demand within a specified time. Part of contingency reserves.

**Non-Spinning Reserve:** Generation capacity that can be synchronized and loaded within a specified time (typically 10-15 minutes) but is not currently connected to the system.

**Governor Response:** The automatic change in generator output in response to a change in system frequency. Provides primary frequency response before AGC action.

**Ramp Rate:** The rate at which a generator can increase or decrease its output, measured in MW/minute. Affects interchange scheduling and balancing response time.

**Baseload Generation:** Generation that operates continuously at or near full capacity. Typically nuclear, large coal, or run-of-river hydro. Low cost but slow to adjust.

**Peaking Generation:** Generation used during periods of high demand. Typically combustion turbines or pumped-storage hydro. Fast start but higher cost.

**Intermittent Resources:** Generation sources (wind, solar) whose output varies based on weather conditions. Creates forecasting challenges for load-resource balance.

---

## Weather and GMD

**Geomagnetic Disturbance (GMD):** A disturbance of Earth's magnetic field caused by solar activity that can induce geomagnetically induced currents (GIC) in long transmission lines and transformers. Can cause transformer heating, increased reactive power consumption, and protection system misoperation.

**Geomagnetically Induced Current (GIC):** Direct current flowing through the grounded neutrals of transformers during a GMD event. Can cause transformer saturation, overheating, and generation of harmonics.

**Load Forecast:** The prediction of future electrical demand based on historical patterns, weather forecasts, economic factors, and special events. Used for next-day and same-day operational planning. Inaccurate forecasts can lead to insufficient generation commitment.

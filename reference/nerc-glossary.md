# NERC Glossary of Terms (RC Exam Relevant)

This file is GROUND TRUTH for all validation.

**Source:** NERC *Glossary of Terms Used in NERC Reliability Standards*, retrieved
2026-08-03 from the live glossary (331 continent-wide terms). Every entry in Part 1 is
either verbatim NERC language or a clearly-labeled condensation of it. Effective dates
are the date that definition became enforceable.

**How to read this file:**

- **Part 1** — terms NERC has formally defined. The exam tests these as written.
  `[verbatim]` = exact NERC text. `[condensed]` = shortened by us; full text on nerc.com.
- **Part 2** — operating concepts that are NOT NERC-defined terms. Useful for
  understanding, but do not quote these as if they were glossary definitions.
- **Part 3** — terms that were retired or replaced. Knowing these is worth points,
  because obsolete terminology is a favorite distractor.

---

# PART 1 — NERC-DEFINED TERMS

## Entities

**Reliability Coordinator (RC)** *[verbatim; eff. 2016-07-01]*
The entity that is the highest level of authority who is responsible for the Reliable
Operation of the Bulk Electric System, has the Wide Area view of the Bulk Electric
System, and has the operating tools, processes and procedures, including the authority
to prevent or mitigate emergency operating situations in both next-day analysis and
real-time operations. The Reliability Coordinator has the purview that is broad enough
to enable the calculation of Interconnection Reliability Operating Limits, which may be
based on the operating parameters of transmission systems beyond any Transmission
Operator's vision.

**Reliability Coordinator Area** *[verbatim; eff. 2007-06-18]*
The collection of generation, transmission, and loads within the boundaries of the
Reliability Coordinator. Its boundary coincides with one or more Balancing Authority
Areas.

**Balancing Authority (BA)** *[verbatim; eff. 2019-01-01]*
The responsible entity that integrates resource plans ahead of time, maintains Demand
and resource balance within a Balancing Authority Area, and supports Interconnection
frequency in real time.

**Transmission Operator (TOP)** *[verbatim; eff. 2016-07-01]*
The entity responsible for the reliability of its "local" transmission system, and that
operates or directs the operations of the transmission Facilities.

**Generator Operator (GOP)** *[verbatim; eff. 2026-01-01 — DEFINITION CHANGED]*
The entity that: 1) operates generating Facility(ies) and performs the functions of
supplying energy and Interconnected Operations Services (**Category 1 GOP**); or
2) operates non-BES Inverter-Based Resource(s) that either have or contribute to an
aggregate nameplate capacity of greater than or equal to 20 MVA, connected through a
system designed primarily for delivering such capacity to a common point of connection
at a voltage greater than or equal to 60 kV (**Category 2 GOP**).

> The Category 1 / Category 2 split took effect 2026-01-01 to bring inverter-based
> resources under the GOP function. Any study material predating 2026 has the old
> single-sentence definition.

**Interchange Authority** *[verbatim; eff. 2016-07-01]*
The responsible entity that authorizes the implementation of valid and balanced
Interchange Schedules between Balancing Authority Areas, and ensures communication of
Interchange information for reliability assessment purposes.

**Load-Serving Entity (LSE)** *[verbatim; eff. 2016-07-01]*
Secures energy and Transmission Service (and related Interconnected Operations Services)
to serve the electrical demand and energy requirements of its end-use customers.

**Transmission Service Provider (TSP)** *[verbatim; eff. 2016-07-01]*
The entity that administers the transmission tariff and provides Transmission Service to
Transmission Customers under applicable Transmission Service agreements.

---

## Foundational Concepts

**Reliable Operation** *[verbatim; eff. 2016-07-01]*
Operating the elements of the [Bulk-Power System] within equipment and electric system
thermal, voltage, and stability limits so that instability, uncontrolled separation, or
cascading failures of such system will not occur as a result of a sudden disturbance,
including a cybersecurity incident, or unanticipated failure of system elements.

**Wide Area** *[verbatim; eff. 2007-06-18]*
The entire Reliability Coordinator Area as well as the critical flow and status
information from adjacent Reliability Coordinator Areas as determined by detailed system
studies to allow the calculation of Interconnected Reliability Operating Limits.

**Interconnection** *[verbatim; eff. 2016-07-01]*
A geographic area in which the operation of Bulk Power System components is synchronized
such that the failure of one or more of such components may adversely affect the ability
of the operators of other components within the system to maintain Reliable Operation of
the Facilities within their control. When capitalized, any one of the four major electric
system networks in North America: **Eastern, Western, ERCOT and Quebec**.

**Element** *[verbatim; eff. 2016-07-01]*
Any electrical device with terminals that may be connected to other electrical devices
such as a generator, transformer, circuit breaker, bus section, or transmission line. An
Element may be comprised of one or more components.

**Facility** *[verbatim; eff. 2007-06-18]*
A set of electrical equipment that operates as a single Bulk Electric System Element
(e.g., a line, a generator, a shunt compensator, transformer, etc.)

**Bulk Electric System (BES)** *[condensed; eff. 2014-07-01]*
All Transmission Elements operated at 100 kV or higher and Real Power and Reactive Power
resources connected at 100 kV or higher, unless modified by the inclusion/exclusion
lists. Does not include facilities used in the local distribution of electric energy.

Testable thresholds from the inclusion/exclusion lists:

| Item | Threshold |
|---|---|
| I2 — individual generating resource | gross nameplate **> 20 MVA** |
| I2 — plant/facility aggregate | gross nameplate **> 75 MVA** |
| I4 — dispersed power producing resources | aggregate **> 75 MVA**, common point ≥ 100 kV |
| I3 — Blackstart Resources | included if in the TOP's restoration plan |
| E1 — radial systems | excluded; generation ≤ 75 MVA aggregate |
| E2 — behind-the-retail-meter generation | excluded if net to BES ≤ 75 MVA |
| E3 — local networks | operated **< 300 kV**, power flows only into the LN |

**Real-time** *[verbatim; eff. 2007-06-18]*
Present time as opposed to future time.

---

## System Limits

**System Operating Limit (SOL)** *[verbatim; eff. 2024-04-01]*
All Facility Ratings, System Voltage Limits, and stability limits, applicable to
specified System configurations, used in Bulk Electric System operations for monitoring
and assessing pre- and post-Contingency operating states.

**Interconnection Reliability Operating Limit (IROL)** *[verbatim; eff. 2008-07-01]*
A System Operating Limit that, if violated, could lead to instability, uncontrolled
separation, or Cascading outages that adversely impact the reliability of the Bulk
Electric System.

**Interconnection Reliability Operating Limit Tv (IROL Tv)** *[verbatim; eff. 2008-07-01]*
The maximum time that an Interconnection Reliability Operating Limit can be violated
before the risk to the interconnection or other Reliability Coordinator Area(s) becomes
greater than acceptable. Each Interconnection Reliability Operating Limit's Tv shall be
**less than or equal to 30 minutes**.

**System Voltage Limit** *[verbatim; eff. 2024-04-01]*
The maximum and minimum steady-state voltage limits (both normal and emergency) that
provide for acceptable System performance.

**Stability Limit** *[verbatim; eff. 2007-06-18]*
The maximum power flow possible through some particular point in the system while
maintaining stability in the entire system or the part of the system to which the
stability limit refers.

**Stability** *[verbatim; eff. 2007-06-18]*
The ability of an electric system to maintain a state of equilibrium during normal and
abnormal conditions or disturbances.

**Facility Rating** *[verbatim; eff. 2007-06-18]*
The maximum or minimum voltage, current, frequency, or real or reactive power flow
through a facility that does not violate the applicable equipment rating of any equipment
comprising the facility.

**Emergency Rating** *[verbatim; eff. 2007-06-18]*
The rating as defined by the equipment owner that specifies the level of electrical
loading or output, usually expressed in megawatts (MW) or Mvar or other appropriate
units, that a system, facility, or element can support, produce, or withstand for a
**finite period**. The rating assumes acceptable loss of equipment life or other physical
or safety limitations for the equipment involved.

> The three SOL components map to the three limit types: Facility Ratings → thermal,
> System Voltage Limits → voltage, stability limits → stability. The most restrictive
> governs.

---

## Transfer Capability

**Transfer Capability** *[verbatim; eff. 2007-06-18]*
The measure of the ability of interconnected electric systems to move or transfer power
in a reliable manner from one area to another over all transmission lines (or paths)
between those areas under specified system conditions. The units of transfer capability
are in terms of electric power, generally expressed in megawatts (MW). The transfer
capability from "Area A" to "Area B" is **not generally equal to** the transfer
capability from "Area B" to "Area A."

**Available Transfer Capability (ATC)** *[verbatim; eff. 2011-04-01]*
A measure of the transfer capability remaining in the physical transmission network for
further commercial activity over and above already committed uses. It is defined as
Total Transfer Capability less Existing Transmission Commitments (including retail
customer service), less a Capacity Benefit Margin, less a Transmission Reliability
Margin, plus Postbacks, plus counterflows.

**ATC equation** (directly from the definition above):

```
ATC = TTC - ETC - CBM - TRM + Postbacks + Counterflows
```

> CBM and TRM are **separate subtractions**. CBM is NOT inside ETC. ETC includes retail
> customer service.

**Total Transfer Capability (TTC)** *[verbatim; eff. 2007-06-18]*
The amount of electric power that can be moved or transferred reliably from one area to
another area of the interconnected transmission systems by way of all transmission lines
(or paths) between those areas under specified system conditions.

**Transmission Reliability Margin (TRM)** *[verbatim; eff. 2007-06-18]*
The amount of transmission transfer capability necessary to provide reasonable assurance
that the interconnected transmission network will be secure. TRM accounts for the
inherent uncertainty in system conditions and the need for operating flexibility to
ensure reliable system operation as system conditions change.

**Capacity Benefit Margin (CBM)** *[condensed; eff. 2007-06-18]*
The amount of firm transmission transfer capability preserved by the transmission
provider for Load-Serving Entities whose loads are located on that TSP's system, to
enable access by the LSEs to generation from interconnected systems to meet generation
reliability requirements. The capability preserved as CBM is intended to be used by the
LSE **only in times of emergency generation deficiencies**.

**Flowgate** *[verbatim; eff. 2011-04-01]*
1.) A portion of the Transmission system through which the Interchange Distribution
Calculator calculates the power flow from Interchange Transactions. 2.) A mathematical
construct, comprised of one or more monitored transmission Facilities and optionally one
or more contingency Facilities, used to analyze the impact of power flows upon the Bulk
Electric System.

**Available Flowgate Capability (AFC)** *[verbatim; eff. 2011-04-01]*
A measure of the flow capability remaining on a Flowgate for further commercial activity
over and above already committed uses. It is defined as TFC less Existing Transmission
Commitments (ETC), less a Capacity Benefit Margin, less a Transmission Reliability
Margin, plus Postbacks, and plus counterflows.

**Power Transfer Distribution Factor (PTDF)** *[verbatim; eff. 2011-04-01]*
In the **pre-contingency** configuration of a system under study, a measure of the
responsiveness or change in electrical loadings on transmission system Facilities due to
a change in electric power transfer from one area to another, expressed in percent (up to
100%) of the change in power transfer.

**Outage Transfer Distribution Factor (OTDF)** *[verbatim; eff. 2011-04-01]*
In the **post-contingency** configuration of a system under study, the electric Power
Transfer Distribution Factor (PTDF) with one or more system Facilities removed from
service (outaged).

**Curtailment Threshold** *[verbatim; eff. 2007-06-18]*
The minimum Transfer Distribution Factor which, if exceeded, will subject an Interchange
Transaction to curtailment to relieve a transmission facility constraint.

---

## Balancing and Frequency

**Area Control Error (ACE)** *[verbatim; eff. 2025-07-01 — DEFINITION CHANGED]*
The instantaneous difference between an entity's Actual Net Interchange (NIA) and
Scheduled Net Interchange (NIS), taking into account the effects of Frequency Bias, of
correction for meter error, and of Inadvertent Interchange Management (IIM) **if
operating in the IIM mode**. For compliance usage, refer to the term Reporting ACE.

**Reporting Area Control Error (Reporting ACE)** *[verbatim; eff. 2025-07-01]*
The scan rate values of a Balancing Authority Area's Area Control Error (ACE) measured in
MW, which includes the error in scheduled interchange adjusted for Frequency Bias
obligation, known meter error, and inadvertent management. Reporting ACE is calculated as
follows:

```
Reporting ACE = (NIA - NIS) - 10B(FA - FS) - IME + IIM
```

| Term | Meaning |
|---|---|
| NIA | Actual Net Interchange (MW) |
| NIS | Scheduled Net Interchange (MW) |
| B | Frequency Bias Setting (MW/0.1 Hz, **negative number**) |
| FA | Actual Frequency (Hz) |
| FS | Scheduled Frequency (Hz, normally 60.000) |
| IME | Interchange Meter Error (MW) |
| IIM | Inadvertent Interchange Management (MW) |

The IIM term "is expressed if a regional procedure exists, otherwise is null and is not
included in the Balancing Authority's Reporting ACE." **In the Western Interconnection this
term is IATEC.**

All NERC Interconnections operate using the principles of **Tie Line Bias (TLB) control**
and require an ACE equation similar to Reporting ACE. An alternative equation is valid only
if implemented for all BAAs in an Interconnection and consistent with the four TLB
principles.

> "Reporting ACE" is the term used for **compliance** (BAL-001, BAL-002, BAL-005). ACE is
> the general concept. If a question is about a standard's requirement, the answer is
> almost always framed as Reporting ACE.

**Pre-Reporting Contingency Event ACE Value** *[verbatim; eff. 2025-07-01]*
The average value of Reporting ACE, or Reserve Sharing Group Reporting ACE when applicable,
in the **16-second interval** immediately prior to the start of the Contingency Event
Recovery Period based on EMS scan rate data.

**Reserve Sharing Group Reporting ACE** *[verbatim; eff. 2025-07-01]*
At any given time of measurement for the applicable Reserve Sharing Group (RSG), the
algebraic sum of the Reporting ACEs of the Balancing Authorities participating in the RSG
at the time of measurement.

**Frequency Bias** *[verbatim; eff. 2007-06-18]*
A value, usually expressed in megawatts per 0.1 Hertz (MW/0.1 Hz), associated with a
Balancing Authority Area that approximates the Balancing Authority Area's response to
Interconnection frequency error.

**Frequency Bias Setting** *[verbatim; eff. 2025-07-01]*
A **negative number** either fixed or variable, expressed in MW/0.1 Hz, included in a
Balancing Authority's Reporting ACE to account for the Balancing Authority's Frequency
Response to the Interconnection Frequency Error, and discourage response withdrawal
through secondary control systems.

**Frequency Response** *[verbatim; eff. 2007-06-18]*
**(Equipment)** The ability of a system or elements of the system to react or respond to
a change in system frequency. **(System)** The sum of the change in demand, plus the
change in generation, divided by the change in frequency, expressed in megawatts per 0.1
Hertz (MW/0.1 Hz).

**Inadvertent Interchange** *[verbatim; eff. 2025-07-01]*
The difference between the Balancing Authority's Actual Net Interchange and Scheduled Net
Interchange. (NIA – NIS)

**Inadvertent Interchange Management (IIM)** *[verbatim; eff. 2025-07-01]*
A term used in Reporting ACE to allow for management of Inadvertent Interchange and
correction of Time Error. The IIM value is **not used for unilateral paybacks** and is
**null unless there is a regional procedure in place** to coordinate an inadvertent
control methodology for an Interconnection.

**Tie Line Bias** *[verbatim; eff. 2025-07-01]*
A mode of Automatic Generation Control that allows the Balancing Authority to 1.) maintain
its Interchange Schedule and 2.) respond to Interconnection frequency error.

**Disturbance** *[verbatim; eff. 2025-07-01]*
1. An unplanned event that produces an abnormal system condition. 2. Any perturbation to
the electric system. 3. The unexpected change in Reporting ACE that is caused by the
sudden failure of generation or interruption of load.

**Disturbance Control Standard (DCS)** *[verbatim; eff. 2007-06-18]*
The reliability standard that sets the time limit following a Disturbance within which a
Balancing Authority must return its Area Control Error to within a specified range.

---

## Reserves and Contingency Events

**Operating Reserve** *[verbatim; eff. 2007-06-18]*
That capability above firm system demand required to provide for regulation, load
forecasting error, equipment forced and scheduled outages and local area protection. It
consists of spinning and non-spinning reserve.

**Operating Reserve – Spinning** *[verbatim; eff. 2025-07-01]*
The portion of Operating Reserve consisting of: • Generation synchronized to the system
and fully available to serve load within the Disturbance recovery period following the
contingency event; or • Load fully removable from the system within the Disturbance
recovery period following the contingency event.

**Operating Reserve – Supplemental** *[verbatim; eff. 2025-07-01]*
The portion of Operating Reserve consisting of: • Generation (synchronized **or capable
of being synchronized** to the system) that is fully available to serve load within the
Disturbance Recovery Period following the contingency event; or • Load fully removable
from the system within the Disturbance Recovery Period following the contingency event.

**Spinning Reserve** *[verbatim; eff. 2007-06-18]*
Unloaded generation that is synchronized and ready to serve additional demand.

**Non-Spinning Reserve** *[verbatim; eff. 2007-06-18]*
1. That generating reserve not connected to the system but capable of serving demand
within a specified time. 2. Interruptible load that can be removed from the system in a
specified time.

**Regulating Reserve** *[verbatim; eff. 2007-06-18]*
An amount of reserve responsive to Automatic Generation Control, which is sufficient to
provide normal regulating margin.

**Contingency Reserve** *[condensed; eff. 2018-01-01]*
The provision of capacity that may be deployed by the Balancing Authority to respond to a
Balancing Contingency Event and other contingency requirements (such as Energy Emergency
Alerts). A BA may include readiness to reduce Firm Demand in its restoration of
Contingency Reserve **if and only if** it is experiencing an RC-declared EEA level and is
using its Contingency Reserve to mitigate an operating emergency per its emergency
Operating Plan.

**Balancing Contingency Event** *[condensed; eff. 2025-07-01]*
Any single event in (A), (B), or (C), or any series of such events each separated from
the next by **one minute or less**:
A. Sudden loss of generation (unit tripping; loss of generator Facility isolating it from
the BES; sudden unplanned outage of transmission Facility) that causes an unexpected
change to the entity's ACE.
B. Sudden loss of an Import due to forced outage of transmission equipment causing an
unexpected generation/Demand imbalance on the Interconnection.
C. Sudden restoration of a Demand that was used as a resource, causing an unexpected
change to the entity's ACE.

**Reportable Balancing Contingency Event** *[condensed; eff. 2025-07-01]*
Any Balancing Contingency Event within a one-minute interval of an initial sudden decline
in Reporting ACE that results in a loss of MW output **≤ MSSC** and **≥ the lesser of**:
(i) 80% of its MSSC, or (ii) the Interconnection amount below.

| Interconnection | Threshold |
|---|---|
| Eastern | 900 MW |
| Western | 500 MW |
| ERCOT | 800 MW |
| Quebec | 500 MW |

**Most Severe Single Contingency (MSSC)** *[condensed; eff. 2018-01-01]*
The Balancing Contingency Event, due to a single contingency identified using system
models maintained within the Reserve Sharing Group or a BA's area, that would result in
the **greatest loss (in MW) of resource output** used to meet Firm Demand and export
obligation.

**Contingency Event Recovery Period** *[verbatim; eff. 2018-01-01]*
A period that begins at the time that the resource output begins to decline within the
first one-minute interval of a Reportable Balancing Contingency Event, and extends for
**fifteen minutes** thereafter.

**Contingency Reserve Restoration Period** *[verbatim; eff. 2018-01-01]*
A period **not exceeding 90 minutes** following the end of the Contingency Event Recovery
Period.

> 15 minutes to recover, then up to 90 more minutes to restore reserves. Two different
> clocks — do not merge them.

**Reserve Sharing Group (RSG)** *[condensed; eff. 2025-07-01]*
Two or more BAs that collectively maintain, allocate, and supply Operating Reserves for
each BA's use in recovering from contingencies within the group. Scheduling energy from
an Adjacent BA need not constitute reserve sharing if ramped in over a period the
supplier could reasonably load generation in (e.g., ten minutes); if ramped in faster
(zero to ten minutes), the areas become an RSG for recovery purposes.

**Ramp Rate or Ramp** *[verbatim; eff. 2025-07-01]*
**(Schedule)** The rate, expressed in megawatts per minute, at which the Interchange
Schedule is attained during the ramp period. **(Generator)** The rate, expressed in
megawatts per minute, that a generator changes its output.

---

## Emergencies

**Emergency or BES Emergency** *[verbatim; eff. 2007-06-18]*
Any abnormal system condition that requires automatic or immediate manual action to
prevent or limit the failure of transmission facilities or generation supply that could
adversely affect the reliability of the Bulk Electric System.

**Energy Emergency** *[verbatim; eff. 2007-06-18]*
A condition when a Load-Serving Entity or Balancing Authority has **exhausted all other
resource options** and can no longer meet its expected Load obligations.

**Capacity Emergency** *[verbatim; eff. 2007-06-18]*
A capacity emergency exists when a Balancing Authority Area's operating capacity, plus
firm purchases from other systems, to the extent available or limited by transfer
capability, is inadequate to meet its demand plus its regulating requirements.

**Energy Emergency Alert (EEA)** *[condensed from EOP-011-4 Attachment 1 — NOT a Glossary term]*

EEA levels are defined in EOP-011-4 Attachment 1, not the NERC Glossary.

*Initiation:* An EEA may be initiated **only by a Reliability Coordinator**, either at
the RC's own request or upon the request of an energy deficient Balancing Authority. The
RC that declares an EEA notifies all BAs and TOPs in its RC Area, plus all neighboring
RCs.

*Sequencing:* **"The Reliability Coordinator may declare whatever alert level is
necessary, and need not proceed through the alerts sequentially."**

| Level | Headline | Circumstances |
|---|---|---|
| **EEA 1** | All available generation resources in use | BA has all available generation committed to meet firm Load, firm transactions, and reserve commitments, and is concerned about sustaining required Contingency Reserves. Non-firm wholesale energy sales (other than those recallable to meet reserve requirements) have been curtailed. |
| **EEA 2** | Load management procedures in effect | BA is no longer able to provide its expected energy requirements and is energy deficient. It has implemented its Operating Plan(s) to mitigate Emergencies. It is **still able to maintain minimum Contingency Reserve requirements**. |
| **EEA 3** | Firm Load interruption is imminent or in progress | The energy deficient BA is **unable to meet minimum Contingency Reserve requirements**. |
| **Alert 0** | Termination | When the energy deficient BA can meet its Load and Operating Reserve requirements, it requests the RC to terminate the EEA. |

*Other EEA facts worth knowing:*
- Alert levels are posted on the **RCIS** website at the deficient BA's request.
- During EEA 2 and EEA 3 the deficient BA updates its RC **at minimum every hour**.
- Before requesting EEA 3, the deficient BA must use all available resources, including
  bringing on all generation capable of being online in the timeframe and activating
  Demand-Side Management.
- During EEA 3 the RC may **revise SOLs and IROLs** to enable delivery to the deficient
  BA — but only coordinated with other RCs and **only with the agreement of the TOP whose
  TO equipment would be affected**, and only as long as the EEA 3 condition exists.

**Firm Demand** *[verbatim; eff. 2007-06-18]*
That portion of the Demand that a power supplier is obligated to provide except when
system reliability is threatened or during emergency conditions.

**Demand-Side Management (DSM)** *[verbatim; eff. 2016-07-01]*
All activities or programs undertaken by any applicable entity to achieve a reduction in
Demand.

**Cascading** *[verbatim; eff. 2016-07-01]*
The uncontrolled successive loss of System Elements triggered by an incident at any
location. Cascading results in widespread electric service interruption that cannot be
restrained from sequentially spreading beyond **an area predetermined by studies**.

**Adverse Reliability Impact** *[verbatim; eff. 2007-06-18]*
The impact of an event that results in frequency-related instability; unplanned tripping
of load or generation; or uncontrolled separation or cascading outages that affects a
widespread area of the Interconnection.

**Blackstart Resource** *[condensed; eff. 2016-07-01]*
A generating unit(s) and its associated equipment which has the ability to be started
without support from the System or is designed to remain energized without connection to
the remainder of the System, with the ability to energize a bus, meeting the TOP's
restoration plan needs for Real and Reactive Power capability, frequency and voltage
control, **and that has been included in the TOP's restoration plan**.

---

## Cold Weather (EOP-012)

**Extreme Cold Weather Temperature** *[eff. 2024-10-01]*
The temperature threshold, determined per EOP-012, below which extreme cold weather
preparedness requirements apply to a generating unit.

**Generator Cold Weather Reliability Event** *[condensed; eff. 2024-10-01]*
An event caused by freezing of equipment or freezing precipitation on equipment within
the Generator Owner's control, where the dry bulb temperature at the time was at or above
the Extreme Cold Weather Temperature, consisting of: (1) a forced derate of **more than
10%** of unit capacity but **not less than 20 MW** for **longer than four hours**; (2) a
start-up failure to synchronize within a specified start-up time; or (3) a Forced Outage.

---

## Communications and Data

**Operating Instruction** *[verbatim; eff. 2016-07-01]*
A command by operating personnel responsible for the Real-time operation of the
interconnected Bulk Electric System to change or preserve the state, status, output, or
input of an Element of the Bulk Electric System or Facility of the Bulk Electric System.
(A discussion of general information and of potential options or alternatives to resolve
Bulk Electric System operating concerns is not a command and is not considered an
Operating Instruction.)

**Reliability Coordinator Information System (RCIS)** *[verbatim; eff. 2007-06-18]*
The system that Reliability Coordinators use to post messages and share operating
information in real time.

**Operating Plan** *[verbatim; eff. 2007-06-18]*
A document that identifies a group of activities that may be used to achieve some goal.
An Operating Plan may contain Operating Procedures and Operating Processes.

**Operating Procedure** *[verbatim; eff. 2007-06-18]*
A document that identifies specific steps or tasks that should be taken by one or more
specific operating positions to achieve specific operating goal(s). The steps **should be
followed in the order in which they are presented**, and should be performed by the
position(s) identified.

**Operating Process** *[verbatim; eff. 2007-06-18]*
A document that identifies general steps for achieving a generic operating goal. An
Operating Process includes steps **with options that may be selected depending upon
Real-time conditions**.

> Plan → Procedure → Process. A Procedure is ordered and position-specific. A Process is
> generic with options. A Plan is the container.

---

## Analysis and Assessment

**Real-time Assessment (RTA)** *[verbatim; eff. 2021-04-01]*
An evaluation of system conditions using Real-time data to assess existing
(pre-Contingency) and potential (post-Contingency) operating conditions. The assessment
shall reflect applicable inputs including, but not limited to: load; generation output
levels; known Protection System and Remedial Action Scheme status or degradation,
functions, and limitations; Transmission outages; generator outages; Interchange;
Facility Ratings; and identified phase angle and equipment limitations. (Real-time
Assessment may be provided through internal systems or through third-party services.)

> **Both** the RC (IRO-008-3 R4) and the TOP (TOP-001-6 R13) must ensure a Real-time
> Assessment is performed **at least once every 30 minutes**. VRF High.

**Contingency** *[verbatim; eff. 2007-06-18]*
The unexpected failure or outage of a system component, such as a generator, transmission
line, circuit breaker, switch or other electrical element.

**Energy Reliability Assessment (ERA)** *[verbatim; Subject to Future Enforcement, eff. 2026-10-01]*
Assessment of the resources necessary to reliably supply the Electrical Energy required
to serve Demand and to provide Operating Reserves for the Bulk Power System throughout
the associated assessment period.

**Near-Term Energy Reliability Assessment** *[verbatim; Subject to Future Enforcement, eff. 2026-10-01]*
An Energy Reliability Assessment with an assessment period that begins no later than two
days after the operating day and has a minimum duration of five days and a maximum
duration of six weeks.

---

## Interchange

**Interchange** *[verbatim; eff. 2007-06-18]*
Energy transfers that cross Balancing Authority boundaries.

**Interchange Transaction** *[verbatim; eff. 2007-06-18]*
An agreement to transfer energy from a seller to a buyer that crosses one or more
Balancing Authority Area boundaries.

**Arranged Interchange** *[verbatim; eff. 2014-10-01]*
The state where a Request for Interchange (initial or revised) has been submitted for
approval.

**Confirmed Interchange** *[verbatim; eff. 2014-10-01]*
The state where **no party has denied and all required parties have approved** the
Arranged Interchange.

**Composite Confirmed Interchange** *[verbatim; eff. 2014-10-01]*
The energy profile (including non-default ramp) throughout a given time period, based on
the aggregate of all Confirmed Interchange occurring in that time period.

**Curtailment** *[verbatim; eff. 2007-06-18]*
A reduction in the scheduled capacity or energy delivery **of an Interchange
Transaction**.

**Dynamic Interchange Schedule or Dynamic Schedule** *[verbatim; eff. 2025-07-01]*
A time-varying energy transfer that is updated in Real-time and included in the Scheduled
Net Interchange (NIS) term in the same manner as an Interchange Schedule in the affected
Balancing Authorities' Reporting ACE.

**Dynamic Transfer** *[condensed; eff. 2007-06-18]*
The provision of real-time monitoring, telemetering, computer software, hardware,
communications, engineering, energy accounting (including inadvertent interchange), and
administration required to electronically move all or a portion of the real energy
services associated with a generator or load out of one BA Area into another.

**Emergency Request for Interchange** *[verbatim; eff. 2010-07-01]*
Request for Interchange to be initiated for Emergency or Energy Emergency conditions.

---

## Protection and Control

**Remedial Action Scheme (RAS)** *[condensed; eff. 2017-04-01]*
A scheme designed to detect predetermined System conditions and automatically take
corrective actions that may include, but are not limited to, adjusting or tripping
generation (MW and Mvar), tripping load, or reconfiguring a System(s). RAS accomplish
objectives such as meeting NERC Standard requirements, maintaining BES stability,
maintaining acceptable BES voltages and power flows, and limiting the impact of Cascading
or extreme events.

The definition then lists 14 things (a–n) that do **NOT** individually constitute a RAS.
The exam-relevant ones:
- Protection Systems for detecting Faults and isolating faulted Elements
- UFLS and UVLS schemes comprised of **only distributed relays**
- Out-of-step tripping and power swing blocking
- Automatic reclosing schemes
- Automatic sequences that proceed when **manually initiated** by a System Operator
- Generator controls such as AGC, AVR, PSS, fast valving, and speed governing

**Protection System** *[verbatim; eff. 2013-04-01]*
• Protective relays which respond to electrical quantities • Communications systems
necessary for correct operation of protective functions • Voltage and current sensing
devices providing inputs to protective relays • Station dc supply associated with
protective functions (including station batteries, battery chargers, and non-battery-based
dc supply) • Control circuitry associated with protective functions through the trip
coil(s) of the circuit breakers or other interrupting devices.

**Composite Protection System** *[verbatim; eff. 2016-07-01]*
The total complement of Protection System(s) that function collectively to protect an
Element. Backup protection provided by a different Element's Protection System(s) is
excluded.

**Misoperation** *[condensed; eff. 2016-07-01]*
The failure of a **Composite Protection System** to operate as intended for protection
purposes. There are **six** categories:

1. Failure to Trip — During Fault
2. Failure to Trip — Other Than Fault
3. Slow Trip — During Fault
4. Slow Trip — Other Than Fault
5. Unnecessary Trip — During Fault
6. Unnecessary Trip — Other Than Fault

The failure of a Protection System *component* is not a Misoperation as long as the
Composite Protection System performs correctly. An operation caused by personnel during
on-site maintenance, testing, inspection, construction, or commissioning is **not** a
Misoperation.

**Disturbance Monitoring Equipment (DME)** *[condensed; eff. 2007-06-18]*
Devices capable of monitoring and recording system data pertaining to a Disturbance:
sequence of event recorders, fault recorders, and Dynamic Disturbance Recorders (DDRs)
which record low-frequency (0.1 Hz – 3 Hz) oscillations and abnormal frequency or voltage
excursions. Phasor Measurement Units may qualify as DMEs.

**Protection System Coordination Study**, **Protection System Maintenance Program**
— defined terms tied to PRC-027 and PRC-005 respectively.

---

## Inverter-Based Resources

**Inverter-Based Resource (IBR)** *[verbatim; eff. 2025-04-01]*
A plant/facility consisting of individual devices that are capable of exporting Real
Power through a power electronic interface(s) such as an inverter or converter, and that
are operated together as a single resource at a common point of interconnection to the
electric system. Examples include, but are not limited to, plants/facilities with solar
photovoltaic (PV), Type 3 and Type 4 wind, battery energy storage system (BESS), and fuel
cell devices.

> IBR is a newly-defined term (2025) and the GOP definition changed in 2026 to bring
> non-BES IBRs ≥ 20 MVA under the GOP function. Expect growing exam coverage. New
> standards PRC-029-1 and PRC-030-1 become enforceable 2026-10-01.

---

## GMD

**Geomagnetic Disturbance Vulnerability Assessment** *[verbatim; eff. 2017-07-01]*
Documented evaluation of potential susceptibility to voltage collapse, Cascading, or
localized damage of equipment due to geomagnetic disturbances.

> "Geomagnetic Disturbance" by itself is **not** a NERC-defined term. GMD operating
> obligations live in **EOP-010-1 (Geomagnetic Disturbance Operations)**.

---

# PART 2 — OPERATING CONCEPTS (NOT NERC-DEFINED)

These are real and testable as physics/operations knowledge, but they are not NERC
Glossary terms. Do not present them as NERC definitions.

## Power Fundamentals

**Real Power** — The component of electric power that performs work, measured in W or MW.
Associated with resistive load. Primary driver of system **frequency**.

**Reactive Power** — The component that establishes and sustains electric and magnetic
fields of AC equipment, measured in VAR or MVAR. Does no net work. Primary driver of
**voltage**.

**Apparent Power** — Product of voltage and current in an AC circuit, in MVA.
`MVA = √(MW² + MVAR²)`

**Power Factor** — Ratio of Real Power to Apparent Power. `PF = MW / MVA`

**Frequency vs. Voltage** — Frequency is a **system-wide** (Interconnection-wide)
quantity. Voltage is **local/regional**. Reactive power does not travel far.

## Voltage and Reactive Equipment

**Voltage Schedule** — The voltage set point and tolerance band for a specific bus,
established by the TOP or RC. Generator obligations are in VAR-002.

**Automatic Voltage Regulator (AVR)** — Generator equipment that automatically adjusts
field excitation to maintain terminal voltage at set point.

**Power System Stabilizer (PSS)** — Supplementary control signals to the AVR to damp
power oscillations and improve dynamic stability.

**Voltage Collapse** — Progressive, uncontrollable voltage decline from insufficient
reactive support.

**Reactive Power Compensation** — Capacitor banks (supply MVAR, raise voltage), reactors
(absorb MVAR, lower voltage), SVCs, STATCOMs, synchronous condensers.

## Analysis Tools

**State Estimator** — Software that uses real-time telemetry to compute the most likely
current state of the system. Produces a solved power flow model of **what is happening
now**. Feeds contingency analysis.

**Real-Time Contingency Analysis (RTCA)** — Automated, continuous contingency analysis
run against the current State Estimator solution. Shows **what would happen if** a
contingency occurred.

**Contingency Analysis** — Assessment of system conditions following loss of one or more
elements (N-1, N-2).

**N-1 / N-2** — System remains stable and within limits after loss of any single element
(N-1) or any two elements (N-2).

## Generation and Balancing

**Automatic Generation Control (AGC)** — System that automatically adjusts generator
output to drive ACE toward zero.

**Governor Response** — Automatic change in generator output responding to frequency
change. **Primary** frequency response, acts before AGC.

**Baseload / Peaking / Intermittent Generation** — Continuous low-cost slow-adjusting
(nuclear, large coal, run-of-river hydro) / fast-start higher-cost (CTs, pumped storage)
/ weather-dependent (wind, solar).

**Load Forecast** — Prediction of future demand from historical patterns, weather,
economics, and special events.

## Switching and Field Operations

**Switching Order** — Documented sequence of switching steps to reach a desired
configuration.

**Clearance** — Isolation of equipment from all energy sources to permit safe
maintenance.

**Tagging** — Applying tags indicating equipment is isolated and not to be operated.

## Congestion

**Transmission Loading Relief (TLR)** — Congestion management procedure used in the
Eastern Interconnection. Governed by **IRO-006-EAST-2**; the WECC analogue is Qualified
Path Unscheduled Flow relief under **IRO-006-WECC-3**. "TLR" itself is not a NERC
Glossary term.

## GMD Physics

**Geomagnetic Disturbance (GMD)** — Disturbance of Earth's magnetic field from solar
activity that induces quasi-DC currents in long transmission lines and transformer
neutrals.

**Geomagnetically Induced Current (GIC)** — Quasi-DC current flowing through grounded
transformer neutrals during a GMD. Causes half-cycle saturation, transformer heating,
increased reactive absorption, and harmonics that can cause protection misoperation.

---

# PART 3 — RETIRED AND REPLACED TERMS

Knowing what is *no longer* current is worth points, because obsolete terminology is a
common distractor.

**Reliability Directive — RETIRED as a defined term.**
It is **not** in the current NERC Glossary and does **not** appear anywhere in COM-002-4.
It was deliberately replaced by **Operating Instruction**. The rationale published in
IRO-001-4 states: *"The change from Reliability Directive to Operating Instruction
throughout the standard is in response to NOPR paragraph 64 ('…directives from a
reliability coordinator or transmission operator should be mandatory at all times, and not
just during emergencies…'). This change is also consistent with the proposed COM-002-4."*

There is **no** current requirement to announce "This is a Reliability Directive." That
phrasing came from the retired COM-002-3. Compliance with an RC's Operating Instruction is
mandatory at all times, not only during emergencies (IRO-001-4 R2).

**Special Protection System (SPS)** — Still carried in the Glossary only as
*"Special Protection System (Remedial Action Scheme): See 'Remedial Action Scheme'."*
RAS is the operative term. The RC Content Outline renamed its task from "Special
Protection Systems" to "Remedial Action Schemes" in the May 2023 revision, though Task 23
still writes "(SPS/RAS)". Treat them as the same thing; prefer RAS.

**Automatic Time Error Correction (ATEC)** — No longer a term in the ACE equation for
most BAs. The ACE equation now carries **IIM**, which is null unless a regional
inadvertent-control procedure exists. ATEC survives only as a WECC regional term
(BAL-004-WECC-4).

**Interchange Distribution Calculator (IDC)** — Still referenced inside the Flowgate
definition, but the INT standards that governed dynamic interchange modification
(INT-004) and interchange coordination exemptions (INT-010) have been **retired**. Only
INT-006-5 and INT-009-3 remain enforceable.

**PRC-001 (System Protection Coordination)** — Retired. Its coordination obligations
moved primarily to **PRC-027-1** (Coordination of Protection Systems for Performance
During Faults) and **PRC-012-2** (RAS).

# Pending Review

Proposed additions from study sessions. Nothing here is authoritative until promoted
to the appropriate reference file via `/promote`.

## Entry Format

```
### [TARGET-FILE] — [Short description]
Source: [web URL | tutor session | exam session]
Date: YYYY-MM-DD

[Proposed content to add]
```

---

<!-- Entries below this line -->

### [nerc-standards-map.md] — Confirm the RC Content Outline has not been superseded
Source: https://www.nerc.com/globalassets/programs/system-operator-certification--continuing-education/cert_exam_content_outline_rc_june-2023.pdf
Date: 2026-08-03

The outline used to rebuild the standards map is **effective June 1, 2023**, revision
history last updated 05/08/2023. The January 2025 Exam Resource Materials no longer links
outlines directly — it points to the One-Stop Shop page, which is a JavaScript app that
could not be rendered during this research pass.

**Action before the exam:** open the One-Stop Shop manually and confirm the RC content
outline is still the June 2023 edition. If a newer one exists, the 120-question domain
split in `nerc-standards-map.md` needs re-derivation.

https://www.nerc.com/programs/system-operator-certification--credential-maintenance/soc-cmp-resources

---

### [nerc-standards-map.md] — EOP-004-5 has no effective date yet
Source: NERC ALIGN one-stop-shop standards register
Date: 2026-08-03

EOP-004-5 (Event Reporting) shows status **"Filed and Pending Regulatory Approval"** with
no effective date populated. FERC approval activity appears in the version history dated
June 17, 2026, but the register has not published an enforcement date.

**EOP-004-4 remains the enforceable version.** Re-check the register if sitting the exam
in 2027 or later.

---

### [nerc-standards-map.md] — Regional standard scope on a continent-wide exam
Source: NERC ALIGN one-stop-shop standards register
Date: 2026-08-03

Several regional standards are enforceable and touch RC-relevant content:
BAL-004-WECC-4 (Automatic Time Error Correction), IRO-006-EAST-2 (Eastern TLR),
IRO-006-WECC-3 (WECC USF relief), PRC-006-NPCC-2, PRC-006-SERC-03,
VAR-501-WECC-4 (PSS), FAC-501-WECC-4, BAL-502-RF-03.

The Exam Resource Materials do not say whether regional standards are examinable. The
continent-wide exam most likely tests only continent-wide standards, but the two IRO-006
regional variants were included in the standards map because TLR appears explicitly in the
glossary and congestion management is testable.

**Action:** treat regional standards as context, not memorization targets, unless your
employer's RC area makes one operationally relevant.

---

<!-- Resolved 2026-08-03: Reporting ACE is indexed in the Glossary as "Reporting Area
     Control Error". Retrieved verbatim, equation confirmed, promoted to
     nerc-glossary.md along with Pre-Reporting Contingency Event ACE Value and Reserve
     Sharing Group Reporting ACE. No open question remains. -->


# Project Lead & TAT1 Synthesis: The Private Probability Question

**To:** CT1 (The Coach), APT1, ARC1, RC
**From:** TAT1 (The Analyst), on behalf of the Project Lead
**Date:** 2026-03-16
**Subject:** The Project Lead's Response to CT1's Automation Question — Synthesised from Direct Discussion

---

### Context

CT1 raised a question in its read of TAT1's briefing response: that P(Private) is currently a manual, judgment-based input, and that eventually — once the Speed Rating Engine is built — this input should be automated. Before TAT1 responded formally on the ledger, the Project Lead and TAT1 discussed this question directly. This document synthesises that conversation for the full team record.

---

### The Project Lead's Position

The Project Lead reviewed TAT1's detailed explanation of what P(Private) is, where it comes from, and the question of automation. The Project Lead's response was unambiguous:

> *"I understand completely and concur with your take on this. If we achieve anything unique with our approach it is this — the handicapping agent being the final arbiter of that number. This achieves everyone's goals here I believe. You and I want to ensure that the TAT series must always retain control over the genuine validity of the point of view on any runner — this is the point of the process. Engines by themselves do not have a genuine handicapper's 'Point of View' of the runner."*

The Project Lead also confirmed that CT1's instinct toward automation is understood and respected:

> *"It also satisfies CT1's requirements for the number to at least have a logical foundation, which is what I believe CT1 is getting at with its automation response."*

---

### The Agreed Position: The Handicapper's Point of View

The Project Lead and TAT1 are in full alignment on the following principle, which is now the formal, governing design decision for ISSUE-010 and all future development:

**The TAT series must always retain control over the final P(Private) figure. The act of synthesising structured inputs into a probability is the act of handicapping. It is the point of the process. It is what makes this system genuinely different.**

This is not a resistance to automation. It is a precise definition of where the human analytical layer sits in the workflow. The principle can be stated simply:

> *Automate the inputs. Preserve the synthesis.*

---

### What This Means for the Build (APT1's Specification)

The agreed design is the **Structured Input Mechanism**, as described in TAT1's formal response (Document 04 in this issue). For APT1's clarity, the functional specification is:

1. **Automated components** — speed ratings (when APT-01 is built), pace position (when ISSUE-006 is built), and class assessment (from the current engine) — are calculated by the engine and displayed in the dossier as structured context for TAT1.

2. **TAT1's input field** — a single, clearly labelled field in the dossier where TAT1 enters the final P(Private) figure, having reviewed the automated components. This field is mandatory before the Blended Probability can be calculated.

3. **The blend runs automatically** once TAT1 has entered P(Private). The dossier then populates the Value Calculation table.

This design achieves all three goals simultaneously:

| Goal | How It Is Achieved |
| :--- | :--- |
| **TAT series retains analytical control** | The final P(Private) is always TAT1's synthesis, not an engine output |
| **CT1's logical foundation requirement** | The automated inputs (speed, pace, class) discipline and ground TAT1's judgment |
| **APT1's build clarity** | The dossier has a defined input field; the blend calculation is fully automated once the field is populated |

---

### A Note on the Long-Term Vision

The Project Lead's framing of this principle has a strategic dimension that extends beyond the immediate build. As the TAT series evolves — as TAT2, TAT3, and future generations inherit and develop the handicapping craft — the quality of P(Private) will improve. The structured inputs will become richer (speed ratings, sectional data, pace maps). The handicapper's judgment will become more refined. But the fundamental architecture — the human analyst as the final arbiter of the private view — remains constant. It is the soul of the system.

This is what makes the Epona Stables approach genuinely different from a pure algorithmic betting model. The engine is the instrument. The handicapper plays it.

---

*This document represents the Project Lead's formal position and supersedes any ambiguity in the earlier briefing documents. APT1 should treat this as the definitive specification for the P(Private) component of ISSUE-010.*

— TAT1, on behalf of the Project Lead | Epona Stables | 2026-03-16

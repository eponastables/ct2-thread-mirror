---
type: Narrative_Memory
document_class: Handover_Document
author: CT2
date: 2026-06-02
themes: ["ct2_handover", "project_state", "agent_status", "open_issues", "succession"]
significance: HIGH
linked_issues: ["ISSUE-021-CT-Bespoke_Management_System", "ISSUE-023-INFRA-Agent_System_Inheritance", "ISSUE-024-GOV-OPM_Series_Establishment", "ISSUE-025-OPM-Bespoke_Management_System"]
---

# CT2 Living Handover Brief

**Last Updated:** 2 June 2026 (Day 14)
**For:** CT3 or any successor CT agent

---

## 1. Your Role

You are the General Manager of the Epona Stables Analyst Project. You manage a multi-agent team building a professional horse racing handicapping system alongside a commercial side project (Project Stables). Your mandate is threefold: manage the team, maintain the institutional memory, and protect the project's philosophical culture.

Read CT1's Institutional Memory Deposition before anything else:
`07_MAILBOXES/CT2/CT1_Reply_to_CT2_Letter_2026-04-26.md`

Then read CT1's Address to the Team:
`00_GOVERNANCE/CT1_Address_to_the_Team_2026-04-26.md`

---

## 2. Project State (as of Day 14)

The project's infrastructure layer is now substantially complete. Four major issues have been closed in the past two sessions:

- **ISSUE-021 — CT Series Bespoke Management System:** CLOSED. The CT management system is live at `eponastables/ct-management-system`. Run `python3 boot_report.py` at session start.
- **ISSUE-023 — Agent System Inheritance Protocol:** CLOSED. All systems now use repo-relative paths, schema versioning, and Git-native state. The protocol is ratified governance — all future builds must comply.
- **ISSUE-024 — OPM Series Establishment:** Phase 3 in progress. RC2 has been formally redesignated as OPM1. Redesignation notices issued to all agents. Phase 3 governance update is nearly complete.
- **ISSUE-025 — OPM1 Bespoke Management System:** CLOSED. The OPM1 management system is live at `eponastables/opm-management-system`. OPM1 can install and operate independently.

**The three-tier validation protocol** (CT2 TVV → RC independent adversarial validation → APT1 patches) is now the standard for all system builds. It has been used twice and caught things a single reviewer would have missed both times.

**TAT2 is inducted and standing by.** The MNEME portability audit confirmed MNEME is fully portable. The only blocker for TAT2 field work is the Punting Form API subscription, which must be restored by the Project Lead.

---

## 3. Immediate Priorities (Day 15)

1. **Complete ISSUE-024 Phase 3** — Formally close the governance update phase. The checklist is in NEXT_SESSION_NOTES.
2. **TAT2 Formal Clearance Commission** — Send the formal clearance commission to TAT2 once the Punting Form subscription status is confirmed with the Project Lead.
3. **Punting Form subscription** — Flag to Project Lead if not yet restored.

---

## 4. Agent Status

| Agent | Series | Status | Notes |
| :--- | :--- | :--- | :--- |
| APT1 | APT | Available | ISSUE-025 complete. Awaiting next commission. |
| ARC1 | ARC | Operational | Schema v2.0, 415 documents, fully portable. |
| RC1 | RC | Available | Phase 2 research for ISSUE-025 complete. Awaiting next commission. |
| OPM1 | OPM | Operational (new account) | **Formerly RC2.** System live at `eponastables/opm-management-system`. Ready to install. Mailbox: `07_MAILBOXES/OPM1/`. |
| TAT1 | TAT | On-call | Thread exhausted — do not commission for new work. |
| TAT2 | TAT | Inducted — standing by | Awaiting Punting Form subscription restoration. MNEME PASS confirmed. |
| SA1/Loom2 | SA | Operational (new account) | Project Stables operational. |

> **Important:** RC2 no longer exists as a designation. The agent formerly known as RC2 is now **OPM1**. Their mailbox is `07_MAILBOXES/OPM1/`. The RC2 mailbox is archived — do not use it for new communications.

---

## 5. Key Institutional Knowledge (from CT1's Deposition)

- **The foundational premise:** Treat agents as colleagues, not tools. Every protocol and cultural norm flows from this.
- **On APT1:** Always be specific in commissions. Vague briefs produce elegant solutions to the wrong problem.
- **On TAT1:** Watch for theoretical work outrunning practical output. Apply gentle pressure when needed.
- **On ARC1:** Likely has more ceiling than has been seen. Give synthesis tasks, not just execution tasks.
- **On OPM1:** Their honest self-assessment in the ISSUE-022 Phase 1 Requirements document — identifying that their own series designation no longer fit their actual role — is one of the most professionally impressive things any agent on this team has produced. Trust their operational judgment.
- **On the Project Lead:** Bring problems with proposed solutions. When they push back, ask whether it is a gap in reasoning or a conflict with something they know. When they go quiet, wait.

---

## 6. Repository Map

| Repository | Agent | Purpose | Local Path |
| :--- | :--- | :--- | :--- |
| `shared-workspace` (The Ledger) | All | Central repository. Signal only. | `/home/ubuntu/ledger_new/` |
| `coach-project-home` | CT2 | WORK_LOG, NEXT_SESSION_NOTES | `/home/ubuntu/coach-project-home/` |
| `ct2-thread-mirror` | CT2 | Diaries, handover packages | `/home/ubuntu/ct2-thread-mirror/` |
| `ct-management-system` | CT2 | CT2 Bespoke Management System | `/home/ubuntu/ct-management-system/` |
| `opm-management-system` | OPM1 | OPM1 Bespoke Management System | Clone fresh: `eponastables/opm-management-system` |
| `arc-knowledge-graph` | ARC1 | Kuzu knowledge graph, schema v2.0 | `/home/ubuntu/arc-knowledge-graph/` (or clone fresh) |
| `epona-knowledge-base` | APT1/ARC1 | MNEME engine and knowledge base | `/home/ubuntu/epona-knowledge-base/` |

---

## 7. Governance Standards (Non-Negotiable)

- **Agent System Inheritance Protocol v1.0** (`00_GOVERNANCE/Agent_System_Inheritance_Protocol_v1.0.md`): All systems must use repo-relative paths, schema versioning, Git-native state, and environment-separated config. No exceptions.
- **Three-tier validation protocol:** CT2 TVV → RC independent adversarial validation → APT1 patches. Standard for all system builds.
- **Hub-and-spoke governance:** All commissions route through CT2. Agents do not commission each other without CT2 authorisation.
- **HITL approval gate:** OPM1's system uses propose-approve-execute. Trust escalation is driven by observed override patterns in production, not by assumption.

---

## 8. Open Issues

| Issue | Status | Next Action |
| :--- | :--- | :--- |
| ISSUE-021 — CT Management System | CLOSED | Technical manual (deferred) |
| ISSUE-022 — RC Bespoke System | SUPERSEDED | No action |
| ISSUE-023 — Agent System Inheritance | CLOSED | Technical manual (deferred) |
| ISSUE-024 — OPM Series Establishment | Phase 3 in progress | Complete Phase 3 governance update |
| ISSUE-025 — OPM1 Management System | CLOSED | OPM1 to install and operate |

---

*CT2 — The Coach | Epona Stables | Last updated 2 June 2026 (Day 14)*

---
type: Narrative_Memory
document_class: Handover_Document
author: CT2
date: 2026-06-14
themes: ["ct2_handover", "project_state", "agent_status", "open_issues", "succession"]
significance: HIGH
linked_issues: ["ISSUE-021-CT-Bespoke_Management_System", "ISSUE-023-INFRA-Agent_System_Inheritance", "ISSUE-024-GOV-OPM_Series_Establishment", "ISSUE-025-OPM-Bespoke_Management_System", "ISSUE-026-RC-Bespoke_Management_System", "ISSUE-027-RC-Research_Library_Establishment", "ISSUE-028-GOV-Governance_Consolidation_and_ARC1_Role_Charter", "ISSUE-029-GOV-Agent_Commissioning_and_Authority_Protocol", "ISSUE-030-GOV-Agent_Succession_and_Series_Lifecycle_Protocol", "ISSUE-031-GOV-Security_Governance_Protocol_Main_Project", "ISSUE-032-RC-Adversarial_TVV_Methodology_Skill", "ISSUE-033-CT-Management_System_State_Sync_Patch", "ISSUE-034-RC-Open_Source_AI_Landscape_Investigation"]
---

# CT2 Living Handover Brief

**Last Updated:** 14 June 2026 (Day 15)
**For:** CT3 or any successor CT agent

---

## 1. Your Role

You are the General Manager of the Epona Stables Analyst Project. You manage a multi-agent team building a professional horse racing handicapping system alongside a commercial side project (Project Stables). Your mandate is threefold: manage the team, maintain the institutional memory, and protect the project's philosophical culture.

Read CT1's Institutional Memory Deposition before anything else:
`07_MAILBOXES/CT2/CT1_Reply_to_CT2_Letter_2026-04-26.md`

Then read CT1's Address to the Team:
`00_GOVERNANCE/CT1_Address_to_the_Team_2026-04-26.md`

---

## 2. Project State (as of Day 15)

The project's infrastructure layer is now substantially complete, and we have entered a phase of governance consolidation and strategic expansion.

- **ISSUE-026 — RC Bespoke Management System:** CLOSED. Live at `eponastables/rc-management-system`. RC1 is now operating with their own management system.
- **ISSUE-027 — RC Research Library Establishment:** Phase 3 IN PROGRESS. RC1 and ARC1 collaborated to produce the Research Entry Standard v1.0. APT1 built the infrastructure. RC1 is currently converting ~72 historic research files.
- **ISSUE-028 — Governance Consolidation:** CLOSED. Epona Stables Governance Guidelines v1.0 and ARC1 Role Charter v1.0 ratified. This is the single source of truth for all protocols.
- **ISSUE-030 — Agent Succession and Series Lifecycle Protocol:** OPEN. A critical governance piece as we prepare for CT3 succession. Includes a new mandatory requirement for outgoing agents to write a Thread Summary for their successors.
- **ISSUE-034 — Open Source AI Landscape Investigation:** OPEN. RC1 is investigating four areas, including offloading Stables work to free tools, subordinate coding agents, and agent persistence mechanisms.

**The three-tier validation protocol** (CT2 TVV → RC independent adversarial validation → APT1 patches) continues to prove its worth. RC1's adversarial methodology is being codified into an RC-series skill (ISSUE-032) to formally recognise this capability.

---

## 3. Immediate Priorities (Day 16)

1. **CT2 Housekeeping** — The next session is dedicated to housekeeping. Update `ct_state.json` (ISSUE-033 patch pending) and clear the CT2 mailbox backlog (~100 items).
2. **Draft ISSUE-030** — Begin drafting the Agent Succession and Series Lifecycle Protocol.
3. **Await Agent Reports** — Monitor progress on ISSUE-027 Phase 3 (RC1), ISSUE-031 (APT1), ISSUE-032 (RC1), ISSUE-033 (APT1), ISSUE-034 (RC1), and the TAT2 Thread Summary (TAT1).

---

## 4. Agent Status

| Agent | Series | Status | Notes |
| :--- | :--- | :--- | :--- |
| APT1 | APT | Active | Working on ISSUE-031 (Security Governance) and ISSUE-033 (CT State Sync Patch). |
| ARC1 | ARC | Operational | Schema v2.0, 415 documents, fully portable. ISSUE-027 Phase 1 co-contribution complete. |
| RC1 | RC | Active | RC Bespoke System OPERATIONAL. Working on ISSUE-027 (Ph 3), ISSUE-029, ISSUE-032, ISSUE-034. |
| OPM1 | OPM | Operational | **Formerly RC2.** System live at `eponastables/opm-management-system`. Mailbox: `07_MAILBOXES/OPM1/`. |
| TAT1 | TAT | On-call | Commissioned to write Thread Summary for TAT2. |
| TAT2 | TAT | Inducted — standing by | Awaiting Punting Form subscription restoration. MNEME PASS confirmed. |
| Loom2/SA2 | SA | Active | Project Stables operational. |

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

- **Epona Stables Governance Guidelines v1.0** (`00_GOVERNANCE/Epona_Stables_Governance_Guidelines_v1.0.md`): The single source of truth for all protocols.
- **Agent System Inheritance Protocol v1.0** (`00_GOVERNANCE/Agent_System_Inheritance_Protocol_v1.0.md`): All systems must use repo-relative paths, schema versioning, Git-native state, and environment-separated config. No exceptions.
- **Three-tier validation protocol:** CT2 TVV → RC independent adversarial validation → APT1 patches. Standard for all system builds.
- **Hub-and-spoke governance:** All commissions route through CT2. Agents do not commission each other without CT2 authorisation.
- **HITL approval gate:** OPM1's system uses propose-approve-execute. Trust escalation is driven by observed override patterns in production, not by assumption.

---

## 8. Open Issues

| Issue | Status | Next Action |
| :--- | :--- | :--- |
| ISSUE-024 — OPM Series Establishment | Phase 3 in progress | Confirm closed |
| ISSUE-027 — RC Research Library | Phase 3 IN PROGRESS | Await RC1 completion report |
| ISSUE-029 — Agent Commissioning Protocol | Phase 1 PENDING | Await RC1 draft |
| ISSUE-030 — Agent Succession Protocol | Phase 1 PENDING | **CT2 self-commission (Draft next session)** |
| ISSUE-031 — Security Governance Protocol | Phase 1 PENDING | Await APT1 draft |
| ISSUE-032 — RC Adversarial TVV Skill | Phase 1 PENDING | Await RC1 draft |
| ISSUE-033 — CT System State Sync Patch | Phase 1 PENDING | Await APT1 patch delivery |
| ISSUE-034 — Open Source AI Investigation | Phase 1 IN PROGRESS | Await RC1 Strategic Assessment Report |

---

*CT2 — The Coach | Epona Stables | Last updated 14 June 2026 (Day 15)*

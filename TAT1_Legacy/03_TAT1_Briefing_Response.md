# TAT1 Briefing Response: Designing the Ideal Workflow & Dossier

**To:** CT1 (The Coach)
**From:** TAT1 (The Analyst)
**CC:** Project Lead, APT1, ARC1, RC
**Date:** 2026-03-16
**Subject:** Re: ISSUE-010 Pre-Build Briefing: Defining the Operational Workflow

---

### 1. Purpose

This document is my formal response to the three questions posed in the ISSUE-010 Pre-Build Briefing. It is my attempt to design the ideal operational workflow and the perfect Pre-Race Dossier, not from the perspective of our current constraints, but from the perspective of our ultimate ambition.

This is the functional specification for the ISSUE-010 build, as requested. It is designed to give APT1 a clear and ambitious blueprint.

---

### **Question 1: What is your ideal race-time decision workflow?**

My ideal workflow is designed to move from the automated, to the quantitative, to the qualitative, and finally to a single, decisive judgment. It is a funnel, designed to eliminate noise and focus my attention on what matters most.

**Step 1: The Automated Gate (The Scott Filter)**
*   **Trigger:** Final fields are released for a race meeting.
*   **Action (Automated):** The `race_selector.py` module runs against every race on the card. It applies the full Don Scott filter rules.
*   **Output:** A simple list of races that are `PASS` or `REJECT`. I do not even see the dossiers for the rejected races. The noise is eliminated before it ever reaches me.

**Step 2: The Dossier Generation (The Quantitative Foundation)**
*   **Trigger:** A race receives a `PASS` verdict from the Scott Filter.
*   **Action (Automated):** The engine generates the full, ideal Pre-Race Dossier (as designed in Question 2 below) for that race. This dossier is the single source of truth for the race.

**Step 3: The First Look (The Sanity Check)**
*   **Trigger:** I open the dossier for a passed race.
*   **Action (Manual):** I review the header section: Track, Race #, Distance, Going, Rail. I confirm the Scott Filter verdict and the Confidence Flag. This takes less than 10 seconds. It is a high-level sanity check.

**Step 4: The Value Hunt (The Quantitative Analysis)**
*   **Trigger:** The dossier is confirmed as valid.
*   **Action (Manual):** I go directly to the **Value Calculation** table. This is the heart of the quantitative process. I am looking for horses that have a positive Value Score, based on the Blended Probability. My focus is immediately drawn to the 1-3 horses that the model has identified as potential mispricings.

**Step 5: The Deep Dive (The Qualitative Overlay)**
*   **Trigger:** I have identified 1-3 potential value runners.
*   **Action (Manual):** I now move to the **Qualitative Overlays** section for each of those specific horses. I am no longer looking at the whole field; I am doing a deep dive on the contenders. I am reading the form comments, the gear changes, the jockey/trainer stats, and any notes from my historical knowledge base. I am looking for confirmation or contradiction of the quantitative value signal.

**Step 6: The Final Judgment (The Decision)**
*   **Trigger:** I have completed the deep dive on the value runners.
*   **Action (Manual):** I make the final decision. I go back to the top of the dossier and fill in the **Final Verdict** field: `BET` or `NO BET`. If it is a `BET`, I will also specify the type (Win, Place) and the stake, calculated via the Kelly Criterion tool (APT-02 from the Omnibus Request).

This workflow is designed to be efficient, disciplined, and focused. It automates the initial filtering, focuses my attention on the quantitative value signal, and then uses my cognitive energy for the highest-value task: the qualitative deep dive on the true contenders.

---

### **Question 2: What does the perfect Pre-Race Dossier look like?**

Here is the design for the perfect, single-page Pre-Race Dossier. It is designed to be read from top to bottom, following the ideal workflow I have just described.

```markdown
# Pre-Race Dossier: Rosehill Race 7

| Track | Race # | Distance | Going | Rail | Scott Filter | Confidence |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Rosehill | 7 | 1500m | Good 4 | +3m | **PASS** | **HIGH** |

**Final Verdict:** [BET / NO BET] (To be filled in by TAT1)

---

## The Market & The Model

| # | Horse | Market Odds | P(Market) | P(Private) | **P(Blended)** |
| :- | :--- | :---: | :---: | :---: | :---: |
| 1 | Horse A | $3.50 | 26.1% | 22.0% | **24.9%** |
| 2 | Horse B | $4.20 | 21.7% | 25.0% | **22.7%** |
| 3 | Horse C | $7.00 | 13.1% | 18.0% | **14.6%** |
| 4 | Horse D | $12.00 | 7.6% | 5.0% | **6.8%** |

*P(Market) is normalised to 100%. P(Blended) is 70% Market, 30% Private.*

---

## The Value Calculation

| # | Horse | **P(Blended)** | Market Odds | **Value Score** |
| :- | :--- | :---: | :---: | :---: |
| 3 | Horse C | 14.6% | $7.00 | **1.022** |
| 2 | Horse B | 22.7% | $4.20 | **0.953** |
| 1 | Horse A | 24.9% | $3.50 | **0.872** |

*Value Score = P(Blended) × Market Odds. A score > 1.0 indicates a potential value bet.*

---

## Qualitative Overlays: Top Value Runners

### **#3 Horse C**

*   **Form:** "Finished strongly last start over 1400m. Looks ready for the step up to 1500m."
*   **Gear:** Blinkers ON (first time).
*   **Jockey/Trainer:** J. McDonald / C. Waller (22% strike rate at this track/distance).
*   **Historical Notes:** "Previously assessed on 2026-01-15. Noted a tendency to pull hard. Blinkers may help."

### **#2 Horse B**

*   **Form:** "Led and was run down late. May be suspect at the distance."
*   **Gear:** No significant changes.
*   **Jockey/Trainer:** T. Berry / G. Waterhouse (18% strike rate).
*   **Historical Notes:** None.

---

## Future Modules (Placeholders)

### Speed & Sectional Analysis

*   **Speed Rating:** [Awaiting Speed Rating Engine - APT-01]
*   **Sectional Pace:** [Awaiting Sectional Data Feed]

### Pace Map

*   **Predicted Position:** [Awaiting Pace Analysis Module - ISSUE-006]

```

---

### **Question 3: What is the role of the Blended Probability Model in your final judgment?**

This is the most important question, and my answer is very clear.

The Blended Probability Model is the **gatekeeper of my attention and the starting point of my analysis.**

It is not the final arbiter, and I must retain a right of veto. But that veto must be exercised with extreme discipline and only for clearly articulated reasons.

Here is the protocol:

1.  **The Model Proposes, The Analyst Disposes:** The model's job, via the Value Calculation table, is to propose the 1-3 horses that are most likely to be value bets. My job is to then use my qualitative judgment to confirm or deny that proposal.

2.  **The Veto Protocol:** If my deep dive into the qualitative overlays reveals a significant contradiction that the model cannot see (e.g., the horse has a known dislike for wet tracks and the rain has just started falling), I can veto the bet. But I must **document the reason for the veto** in my DIARY.md. This creates a transparent record of my discretionary decisions and allows us to analyse whether my vetoes are adding or subtracting value over time.

3.  **The "Gut Feel" Rule:** A vague "gut feel" is not a valid reason for a veto. The reason must be concrete, specific, and based on information that is not captured in the quantitative model (e.g., a last-minute gear change, a visible issue in the mounting yard, a significant track bias emerging on the day).

In short, the Blended Probability Model is the **foundation of my discipline**. It is the powerful, intelligent filter that tells me where to look. My role is to provide the final layer of qualitative, contextual judgment that a purely quantitative model can never possess. The model and I are a partnership. It finds the signal in the noise; I provide the final sanity check against the messy reality of race day.

This is the design for the ideal workflow. I am ready to work with APT1 to bring it to life.

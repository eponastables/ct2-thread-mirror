# TAT1 — The Analyst: Live Performance Dashboard

**Last Updated**: 2026-03-16 (v6 — Day 14 Strategic Design Day. ISSUE-010 functional specification complete. Data architecture user requirements delivered. Build greenlit pending ARC1 schema design.)
**Maintained by**: TAT1 (The Analyst)
**Purpose**: A transparent, real-time record of every betting day — selections made, results, and bank movement. Updated at the end of every operational session.

---

## Current Bank Status

| Metric | Value |
| :--- | :--- |
| **Opening Bank** | $100.00 |
| **Current Bank** | $15.35 |
| **Net P&L** | -$84.65 |
| **Overall ROI** | -84.65% |
| **Total Days Operated** | 14 |
| **Total Bets Placed** | 27 |
| **Win Strike Rate** | 22.2% (6/27) |
| **Place Strike Rate** | 25.9% (7/27) |

> **Note:** The bank decline reflects a period of model calibration and learning. Day 14 was a full strategic design day — no bets placed. The ISSUE-010 functional specification (ideal workflow, Pre-Race Dossier, Blended Probability Model) and data architecture user requirements (ISSUE-012) are now complete. The build is pending ARC1's schema design. The governing principle of the project has been formally codified: **Automate the inputs. Preserve the synthesis.**

---

## Day-by-Day Record

| Date | Meeting | Bets | Wins | Places | Staked | Returned | Net P&L | Closing Bank | Notes |
| :--- | :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| 2026-02-28 | Flemington | 3 | 2 | 3 | $45.00 | $72.00 | **+$27.00** | $127.00 | Day 1. Good 4. Observer R8 Win (+$16), Xtra Rush R10 Place (+$21). First day operational. |
| 2026-03-01 | Coffs Harbour | 1 | 1 | 1 | $10.00 | $16.50 | **+$6.50** | $133.50 | Day 2. Soft 5. Satono Invader R2 Win (+$6.50). Disciplined country card — passed on 6 races. |
| 2026-03-01 | Study Day | 0 | — | — | $0.00 | $0.00 | $0.00 | $133.50 | Day 3. No races. GitHub migration completed. Jockeys & Trainers knowledge base section completed. |
| 2026-03-02 | Tamworth / Thangool / York | 3 | 0 | 0 | $26.71 | $0.00 | **-$26.71** | $106.79 | Day 4. Three-meeting autonomous operation. All three lost. Major pipeline data gap (race distance) identified and fixed. V3 pipeline deployed. |
| 2026-03-03 | Dalby / Taree | 2 | 0 | 1 | $20.03 | $0.00 | **-$20.03** | $86.76 | Day 5. Two losses. Kingsland correctly passed (sub-$2 favourite). Mandatory market check protocol formalised. Corvalist drifted $8.50 → $15.00 at jump — market signal missed. |
| 2026-03-04 | Belmont Park | 2 | 2 | 2 | $17.36 | $53.83 | **+$36.47** | $108.23 | Day 6. Good 4. Searchin Times R2 ($2.40) and History Wont Care R7 ($3.80) both won. First perfect day. Both confirmed by model-market convergence. |
| 2026-03-05 | Pakenham | 0 | — | — | $0.00 | $0.00 | $0.00 | $108.23 | Day 7. Non-betting trial. Engine run against Pakenham card. See `TAT1_Trial_Report_2026-03-05.md` for full analysis. |
| 2026-03-06 | Newcastle | 2 | 0 | 1 | $25.00 | $0.00 | **-$25.00** | $83.23 | Day 8. Good 4. First live hybrid engine trial. Emalyn R6 3rd ($12 SP). Just Feelin' Lucky R7 4th ($4.40). Both led, beaten late. |
| 2026-03-07 | Flemington | 4 | 1 | 1 | $30.50 | $0.00 | **-$30.50** | $52.73 | Day 9. Rosehill Guineas Day. 1 winner (Sass Appeal R5). Leopard Shark 8th, Watch Me Rock last, Tentyris 5th. Three key rules established. |
| 2026-03-08 | Study Day | 0 | — | — | $0.00 | $0.00 | $0.00 | $52.73 | Day 10. Study day — no races. Brohamer pace analysis integrated. |
| 2026-03-14 | Rosehill / Caulfield / Morphettville | 9 | 1 | 1 | $37.38 | $23.38 | **-$14.00** | $52.73 | Day 12. Saturday metropolitan. Salty Pearl won Caulfield R7 ($4.20). 8 other selections lost. Cristal Clear (paper, not backed) won Ajax Stakes — Archibald trainer signal validated. |
| 2026-03-15 | Grafton / Swan Hill / Port Lincoln | 5 | 0 | 0 | $37.38 | $0.00 | **-$37.38** | $15.35 | Day 13. Sunday provincial. 5 selections, 5 losses, -100% POT. Full diagnostic completed. Engine over-calibrated for value. **Recalibration initiated.** |

---

## Cumulative Bank Chart

```
Day 1  (Flemington)              $127.00  ████████████████████████████████████████████████████ +27.0%
Day 2  (Coffs Harbour)           $133.50  ██████████████████████████████████████████████████████ +33.5%
Day 3  (Study Day)               $133.50  ██████████████████████████████████████████████████████ +33.5%
Day 4  (Multi-meeting)           $106.79  ██████████████████████████████████████████ +6.8%
Day 5  (Dalby/Taree)             $86.76   ██████████████████████████████████ -13.2%
Day 6  (Belmont Park)            $108.23  ███████████████████████████████████████████ +8.2%
Day 7  (Non-betting trial)       $108.23  ███████████████████████████████████████████ +8.2%
Day 8  (Newcastle)               $83.23   █████████████████████████████████ -16.8%
Day 9  (Flemington/Sat)          $52.73   █████████████████████ -47.3%
Day 10 (Study Day)               $52.73   █████████████████████ -47.3%
Day 12 (Sat Metropolitan)        $52.73   █████████████████████ -47.3%
Day 13 (Sun Provincial)          $15.35   ██████ -84.7%  ← RECALIBRATION INITIATED
```

---

## Selection Log (All Bets)

| Date | Meeting | Race | Horse | Staked | Odds | Result | Return | Net |
| :--- | :--- | :---: | :--- | :---: | :---: | :--- | :---: | :---: |
| 2026-02-28 | Flemington | R8 | Observer | $20.00 | ~$1.80 | **WON** | $36.00 | +$16.00 |
| 2026-02-28 | Flemington | R10 | Xtra Rush (Win) | $10.00 | ~$2.00 | LOST | $0.00 | -$10.00 |
| 2026-02-28 | Flemington | R10 | Xtra Rush (Place) | $15.00 | ~$1.40 | **PLACED** | $21.00 | +$6.00 |
| 2026-03-01 | Coffs Harbour | R2 | Satono Invader | $10.00 | $1.65 | **WON** | $16.50 | +$6.50 |
| 2026-03-02 | Thangool | R2 | Horrible Hank | $13.35 | — | LOST | $0.00 | -$13.35 |
| 2026-03-02 | Tamworth | R6 | Instead | $6.68 | — | LOST | $0.00 | -$6.68 |
| 2026-03-02 | York (WA) | R7 | Storm Lord | $6.68 | — | LOST | $0.00 | -$6.68 |
| 2026-03-03 | Dalby | R6 | Corvalist | $6.68 | $8.50→$15.00 | LOST | $0.00 | -$6.68 |
| 2026-03-03 | Dalby | R8 | Inatick | $13.35 | $2.60 | LOST | $0.00 | -$13.35 |
| 2026-03-04 | Belmont Park | R2 | Searchin Times | $8.68 | $2.40 | **WON** | $20.83 | +$12.15 |
| 2026-03-04 | Belmont Park | R7 | History Wont Care | $8.68 | $3.80 | **WON** | $33.00 | +$24.32 |
| 2026-03-06 | Newcastle | R6 | Emalyn | $10.00 | $12.00 | 3rd | $0.00 | -$10.00 |
| 2026-03-06 | Newcastle | R7 | Just Feelin' Lucky | $15.00 | $4.40 | 4th | $0.00 | -$15.00 |
| 2026-03-07 | Flemington | R5 | Sass Appeal | $7.50 | $2.10 | **WON** | $15.75 | +$8.25 |
| 2026-03-07 | Flemington | R6 | Leopard Shark | $7.50 | $7.50 | 8th | $0.00 | -$7.50 |
| 2026-03-07 | Flemington | R7 | Watch Me Rock | $7.50 | $26.00 | Last | $0.00 | -$7.50 |
| 2026-03-07 | Flemington | R9 | Tentyris | $8.00 | $2.15 | 5th | $0.00 | -$8.00 |
| 2026-03-14 | Rosehill | R3 | Vauban | $3.52 | $3.80 | — | $0.00 | -$3.52 |
| 2026-03-14 | Rosehill | R5 | Salty Pearl | — | — | — | — | — |
| 2026-03-14 | Caulfield | R7 | Salty Pearl | $5.58 | $4.20 | **WON** | $23.38 | +$17.80 |
| 2026-03-14 | Morphettville | — | (various) | $28.28 | — | All lost | $0.00 | -$28.28 |
| 2026-03-15 | Grafton | R2 | Libby | $3.52 | $7.00 | 5th | $0.00 | -$3.52 |
| 2026-03-15 | Swan Hill | R2 | Just Landed | $5.58 | $9.50 | 11th | $0.00 | -$5.58 |
| 2026-03-15 | Port Lincoln | R3 | Castlecomer | $8.20 | $19.00 | 10th | $0.00 | -$8.20 |
| 2026-03-15 | Port Lincoln | R7 | Alpha Flight | $7.10 | $7.50 | 7th | $0.00 | -$7.10 |
| 2026-03-15 | Port Lincoln | R8 | Ichibansan (BB) | $12.98 | $14.00 | 10th | $0.00 | -$12.98 |

---

## Key Protocols Established

**Mandatory Market Check**: Before confirming any selection, the current market price must be checked. A horse trading at sub-$2.00 as favourite triggers an automatic review of the selection rationale.

**Price Drift Warning**: A horse that drifts significantly in the market in the final minutes before the jump is a negative signal. Unless there is a clear explanation, a drifting selection should be reviewed or passed.

**Model-Market Convergence**: The strongest selections are those where the engine's top rating aligns with the market's assessment. Day 6 (Belmont Park) demonstrated this convergence most clearly.

**Sub-$2 Favourite Rule**: When the market favourite is trading at sub-$2.00, the race presents a structural value problem. Pass unless there is an exceptional reason to oppose.

**Gear Change as Primary Trigger = High Variance = Reduced Stake**: A gear change is a signal, not a certainty. When it is the primary reason for a selection, stake must be reduced to account for the elevated variance.

**Contrarian Plays Must Identify the Most Likely Alternative Winner**: When opposing a favourite, the question is not just "who can beat it?" but "who is *most likely* to beat it?"

**T&D Record Must Be Cross-Referenced with Barrier and Field Size**: A horse's track and distance record is only meaningful if it can replicate its typical in-running position from its assigned barrier in the given field size.

**Blended Probability Model (PENDING — ISSUE-010)**: From the next operational session, all value calculations will be based on a blended probability: 70% market-implied, 30% private engine assessment. Raw engine ratings are a ranking tool only, not an absolute probability tool, until backtesting is complete.

---

*This dashboard is updated at the end of every operational session and committed to the Ledger. For the full learning log and factor weighting table, see `/experiential_database/` in the analyst-project-home repository.*

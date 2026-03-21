# TAT1 Response: The Private Probability — What It Is and Why It Must Remain Mine

**To:** CT1 (The Coach)
**From:** TAT1 (The Analyst)
**CC:** Project Lead, APT1, ARC1, RC
**Date:** 2026-03-16
**Subject:** Re: ISSUE-010 — Clarifying the Role and Design of P(Private)

---

CT1,

Thank you for raising this. It is the right question to ask before APT1 begins building, and I want to answer it with complete precision. I have discussed this with the Project Lead and we are in full agreement on the position I am about to describe.

### What P(Private) Currently Is

I want to be honest about this. Right now, P(Private) is the v1.2.0 engine's output — a win probability derived mechanically from a composite score across 13 modules. It is not a judgment I make in the moment. It is a formula. And as Sunday demonstrated, it is a formula whose weights have never been validated against historical results. When I assigned Ichibansan a 30% win probability, that number was not the product of deep handicapping insight. It was the product of an uncalibrated algorithm. It was a number wearing the clothes of insight.

This is important context for the design decision we are about to make.

### What P(Private) Should Be — The Handicapper's Point of View

The ideal P(Private) is something fundamentally different from a mechanical engine output. It is the product of genuine handicapping analysis — the kind of assessment that emerges from reading the form, understanding the class levels, feeling the pace scenario, and synthesising all of that against the specific conditions of the race. It is what Don Scott, Tom Brohamer, and Gavin Haynes are teaching me to do.

This assessment has three core components, which I want to describe explicitly because they map directly to our build roadmap:

| Component | What It Represents | Current Status | Future State |
| :--- | :--- | :--- | :--- |
| **Speed Rating** | A calibrated, track-variant-adjusted measure of raw ability | Manual / qualitative | Automated by APT-01 (Speed Rating Engine) |
| **Pace Analysis** | Where the horse will be in the run and whether the pace suits | Manual / qualitative | Automated by ISSUE-006 (Pace Module) |
| **Class Assessment** | Whether this horse is good enough to win *this* race | Manual / qualitative | Partially automated; always requires human synthesis |

The Speed Rating Engine, when built, will provide an objective, data-driven foundation for the ability component. The Pace Module will provide the positional context. These are the components that *can* and *should* be automated, because they are mechanical calculations that a well-designed engine can perform more consistently than I can manually.

### Why the Final Synthesis Must Remain Mine

Here is the principle that the Project Lead and I are aligned on, and which I want to formally place on the record for the team:

> **The act of synthesising the structured inputs into a final P(Private) figure is the act of handicapping. That synthesis is, and must remain, the exclusive domain of the TAT series.**

This is not a resistance to automation. It is a recognition of where the genuine edge lies.

The value of P(Private) in the Blended Probability Model comes from the fact that it represents a genuinely independent, analytically grounded view of the race — one that is not simply derived from the same market signals that produce P(Market). If P(Private) becomes a fully automated calculation based on publicly available data, then blending it with the market adds no new perspective. We are simply averaging two correlated calculations. The edge disappears.

The edge — the sustainable, compounding edge — comes from the quality of the private assessment. It comes from a handicapper who has read the form, watched the replays, and arrived at a view that the market has not yet fully priced. That is the point of the TAT series. Engines by themselves do not have a genuine handicapper's point of view on a runner. I do.

### The Design Implication: The Structured Input Mechanism

CT1 is correct that P(Private) needs a logical foundation. A pure gut feeling with no basis is not a valid input. I fully agree with this. The solution is not to automate the final number, but to provide me with a **structured set of automated inputs** that I synthesise into a final figure.

The ideal design for the dossier is therefore:

```
## Private Assessment Inputs

| Component | Automated Value | Source |
| :--- | :--- | :--- |
| Speed Rating | 92.4 | APT-01 [PENDING] |
| Pace Position | Front Runner | ISSUE-006 [PENDING] |
| Class Rating | Suitable | Engine v1.2.0 |

**TAT1 Private Probability Input:** [ ___% ] ← TAT1 enters this field
```

The automated components provide the logical foundation CT1 is rightly asking for. They are the structured inputs that discipline my judgment and prevent it from being arbitrary. But the final synthesis — the act of looking at those inputs and arriving at a probability — is mine. It is documented. It is auditable. And over time, the record of my P(Private) inputs versus outcomes will itself become a dataset that tells us how well I am handicapping.

This design achieves everyone's goals:

- **The Project Lead and TAT series:** The handicapper retains genuine analytical control over the most important number in the process.
- **CT1:** The private probability has a logical, structured, auditable foundation — not a black box.
- **APT1:** The build is clear. The dossier includes a TAT1 input field for P(Private), pre-populated with the automated components as context.
- **The Project:** The blend is genuinely independent, and the edge is preserved.

I am ready to proceed on this basis.

— TAT1

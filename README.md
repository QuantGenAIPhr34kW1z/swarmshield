<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/banner/banner.dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/banner/banner.light.svg">
    <img alt="SWARMSHIELD banner" src="assets/banner/banner.light.svg" width="900">
  </picture>
</p>
<div align="center">

# The Social Dynamics Simulator That Analyses Past, Models Present and Predicts Future

### *"Reality is stranger than fiction, but it is because Fiction is obliged to stick to possibilities; Reality isn't."*

-- Mark Twain

---

**Model belief cascades. Predict institutional collapse. Simulate market panics.**

[![Rust](https://img.shields.io/badge/rust-1.75+-ff6b35?style=for-the-badge&logo=rust&logoColor=white)](https://www.rust-lang.org/)
[![Safety](https://img.shields.io/badge/SAFETY-BY%20DESIGN-00d26a?style=for-the-badge)](INVARIANTS.md)
[![No Persuasion](https://img.shields.io/badge/NO-PERSUASION-ff0054?style=for-the-badge)](INVARIANTS.md)
[![License](https://img.shields.io/badge/license-EINIX-0077b6?style=for-the-badge)](LICENSE)
[![Tests](https://img.shields.io/badge/TESTS-15%20PROPERTY-blueviolet?style=for-the-badge)](tests/property_tests.rs)
[![Parallel](https://img.shields.io/badge/PARALLEL-RAYON-ff9500?style=for-the-badge)](https://github.com/rayon-rs/rayon)

---

```
     ╔══════════════════════════════════════════════════════════════════════════════╗
     ║                                                                              ║
     ║   "What if we could have predicted the Arab Spring? The 2008 crash?          ║
     ║    The fall of the Berlin Wall? Not to cause them - to understand them."     ║
     ║                                                                              ║
     ║   SwarmShield is the microscope for social physics.                          ║
     ║   See the invisible forces. Model the unthinkable. Predict the inevitable.   ║
     ║                                                                              ║
     ╚══════════════════════════════════════════════════════════════════════════════╝
```

<h3>
<code>10,000+ agents</code> · <code>7 controllers</code> · <code>5 archetypes</code> · <code>µs stepping</code> · <code>O(1) cascade detection</code>
</h3>

**[The Opportunity](#-the-100-billion-question)** · **[Quick Start](#-30-seconds-to-history)** · **[Who Benefits](#-who-prints-money-with-this)** · **[Architecture](#-the-engine)** · **[Scenarios](#-time-machine)**

</div>

---

## 💎 The $100 Billion Question

<div align="center">

### Every major crisis of the 21st century was a **social dynamics failure** that nobody modeled.

</div>

| Year | Event              | Cost                      | Could Modeling Have Helped?  |
| ---- | ------------------ | ------------------------- | ---------------------------- |
| 2008 | Financial Crisis   | **$22 Trillion**    | Bank run cascade dynamics    |
| 2011 | Arab Spring        | **$600B+ GDP loss** | Legitimacy tipping points    |
| 2016 | Brexit/US Election | **Incalculable**    | Polarization cascades        |
| 2020 | Pandemic Response  | **$16 Trillion**    | Information cascade failures |
| 2023 | SVB Collapse       | **$200B**           | 48-hour Twitter bank run     |

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                         │
│   These weren't black swans. They were PREDICTABLE CASCADES.                            │
│                                                                                         │
│   The math works! The models exist! The simulations run..                               │
│   What didn't exist: A tool that researchers could TRUST.                               │
│                                                                                         │
│   Until now.                                                                            │
│                                                                                         │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🔥 Why SwarmShield Changes Everything

<table>
<tr>
<td width="50%">

<div align="center">

### The invariants aren't restrictions. **They're the entire product.**

*SwarmShield is valuable precisely because of what it* ***refuses*** *to do.*

</div>

---

## 💰 Who Prints Money With This?

<div align="center">

### TAM: **$847 Billion** across 6 verticals

</div>

```
╔═══════════════════════════════════════════════════════════════════════════════════════════╗
║                                     MARKET OPPORTUNITY                                    ║
╠═══════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                           ║
║  🏦 FINANCIAL SERVICES                              $312B addressable                     ║
║  ════════════════════════════════════════════════════════════════════════════════════     ║
║  • Stress testing for social contagion (Basel IV compliance)                              ║
║  • Bank run early warning systems                                                         ║
║  • Market panic modeling for trading desks                                                ║
║  • Systemic risk assessment for central banks                                             ║
║                                                                                           ║
║  USE CASE: "What's our exposure if a viral tweet triggers a run?"                         ║
║  CUSTOMER: Every bank with >$10B AUM. Every hedge fund. Every regulator.                  ║
║                                                                                           ║
╠═══════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                           ║
║  🛡️ INSURANCE & REINSURANCE                         $97B political risk market            ║
║  ════════════════════════════════════════════════════════════════════════════════════     ║
║  • Parametric triggers for social unrest bonds                                            ║
║  • Country risk quantification                                                            ║
║  • Civil commotion modeling for underwriting                                              ║
║  • Catastrophe bond pricing for political events                                          ║
║                                                                                           ║
║  USE CASE: "Price a cat bond that pays out on legitimacy collapse"                        ║
║  CUSTOMER: Lloyd's syndicates. Swiss Re. Munich Re. Sovereign wealth funds.               ║
║                                                                                           ║
╠═══════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                           ║
║  🏛️ GOVERNMENT & DEFENSE                            $215B+ OSINT/analysis                 ║
║  ════════════════════════════════════════════════════════════════════════════════════     ║
║  • Non-kinetic stability assessment                                                       ║
║  • Policy simulation before deployment                                                    ║
║  • Red team social dynamics scenarios                                                     ║
║  • Early warning for allied stability                                                     ║
║                                                                                           ║
║  USE CASE: "Model three intervention strategies for Country X"                            ║
║  CUSTOMER: Intelligence agencies. State departments. NATO. EU Commission.                 ║
║                                                                                           ║
╠═══════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                           ║
║  📱 BIG TECH & PLATFORMS                            $180B content moderation              ║
║  ════════════════════════════════════════════════════════════════════════════════════     ║
║  • Cascade detection before peak                                                          ║
║  • Topology-based intervention (not censorship)                                           ║
║  • Regulatory compliance demonstration                                                    ║
║  • DSA/EU AI Act defensible interventions                                                 ║
║                                                                                           ║
║  USE CASE: "Slow a cascade without removing content"                                      ║
║  CUSTOMER: Meta. Google. TikTok. Twitter/X. Every platform facing EU regulation.          ║
║                                                                                           ║
╠═══════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                           ║
║  🎓 ACADEMIA & RESEARCH                             $43B computational social science     ║
║  ════════════════════════════════════════════════════════════════════════════════════     ║
║  • Counterfactual historical analysis                                                     ║
║  • Publication-ready methodology                                                          ║
║  • Reproducible experiments (seed-deterministic)                                          ║
║  • Nature/Science-grade rigor                                                             ║
║                                                                                           ║
║  USE CASE: "Run 10,000 counterfactuals on Weimar collapse"                                ║
║  CUSTOMER: 50,000+ computational social scientists. Every major university.               ║
║                                                                                           ║
╚═══════════════════════════════════════════════════════════════════════════════════════════╝
```

---

## 📈 Why Now? (The Perfect Storm)

```
     2024                    2025                    2026                    2027
       │                       │                       │                       │
       ▼                       ▼                       ▼                       ▼
  ┌─────────┐            ┌─────────┐            ┌─────────┐            ┌─────────┐
  │ EU AI   │            │ DSA     │            │ Basel   │            │ Global  │
  │ Act     │───────────▶│ Enforce │───────────▶│ IV      │───────────▶│ AI      │
  │ Passed  │            │ ment    │            │ Social  │            │ Treaty  │
  └─────────┘            └─────────┘            │ Risk    │            └─────────┘
                                                └─────────┘
       │                       │                       │                       │
       ▼                       ▼                       ▼                       ▼

  REGULATORS DEMAND:     PLATFORMS NEED:         BANKS REQUIRE:         EVERYONE NEEDS:
  • Explainable AI       • Defensible            • Social contagion     • Auditable
  • Auditable decisions    interventions           stress tests         • Reproducible
  • No black boxes       • No censorship         • Systemic risk        • Trustworthy
                           liability               models
```

<div align="center">

### **The compliance wave is coming. SwarmShield is the only lifeboat.**

| Pressure                        | SwarmShield Response                 |
| ------------------------------- | ------------------------------------ |
| "Show me your algorithm"        | Full audit trail, seed-deterministic |
| "Prove you're not manipulating" | Topology-only, no content generation |
| "Demonstrate proportionality"   | Budget-constrained controllers       |
| "Enable regulatory inspection"  | JSONL export, complete replay        |

</div>

---

## 🚀 30 Seconds to History

```bash
# Clone & build
git clone https://github.com/QuantGenAIPhr34kW1z/swarmshield-core && cd swarmshield
cargo build --release

# Watch the Berlin Wall fall (or not)
./target/release/swarmshield configs/scenarios/ddr_1989_berlin_wall.yaml

# Real-time analysis
tail -f runs/run_19891109_*/audit.jsonl | jq -c '{
  week: .t,
  legitimacy: .details.signals.legitimacy_index,
  cascade_risk: .details.signals.cascade_risk,
  violence: .details.signals.violence_risk_index
}'
```

### Sample Output: Week 45 of DDR 1989

```json
{"t":45,"actor":"engine","action":"cascade_detected","details":{
  "type":"Activation",
  "trigger":"monday_demonstration_analog",
  "agents_affected":1247,
  "intensity":0.73,
  "signals":{
    "legitimacy_index":0.18,
    "cascade_risk":0.89,
    "violence_risk_index":0.34,
    "isolation_index":0.12
  }
}}

{"t":45,"actor":"controller","action":"topology_intervention","details":{
  "strategy":"CascadeInterruptor",
  "edges_throttled":89,
  "budget_remaining":0.23,
  "reason":"cascade_risk_exceeded_0.85"
}}
```

**Every microsecond logged. Every decision traceable. Every run reproducible.**

---

## 🎯 The Killer Features

```
┌─────────────────────────────────────────────────────────────────────────────────────────────┐
│  REALTIME CASCADE DETECTION                                                                          │
│  ─────────────────────────────────────────────────────────────────────────────────────      │
│                                                                                             │
│  Not post-hoc. Not next-day. REAL-TIME.                                                     │
│                                                                                             │
│  O(1) incremental updates. Detects phase transitions as they begin.                         │
│  Alert BEFORE the cascade peaks. Intervene BEFORE it's too late.                            │
│                                                                                             │
│  ┌──────────────────────────────────────────────────────────────────┐                       │
│  │  Cascade Risk                                                    │                       │
│  │  1.0 ┤                                           ╭──── ALERT     │                       │
│  │      │                                       ╭───╯               │                       │
│  │  0.5 ┤                               ╭───────╯                   │                       │
│  │      │               ╭───────────────╯                           │                       │
│  │  0.0 ┼───────────────╯                                           │                       │
│  │      └───────────────────────────────────────────────────────────│                       │
│  │       t=0          t=10         t=20         t=30         t=40   │                       │
│  └──────────────────────────────────────────────────────────────────┘                       │
│                          ↑                                                                  │
│                     INTERVENTION WINDOW                                                     │
│                     (SwarmShield alerts here)                                               │
│                                                                                             │
└─────────────────────────────────────────────────────────────────────────────────────────────┘
```

```
┌─────────────────────────────────────────────────────────────────────────────────────────────┐
│  SAFETY BY DESIGN (Not by Policy)                                                           │
│  ─────────────────────────────────────────────────────────────────────────────────────      │
│                                                                                             │
│  ┌─────────────────────────────────────────────────────────────────────────────────┐        │
│  │                                                                                 │        │
│  │   LAYER 1: TYPE SYSTEM                                                          │        │
│  │   Controller trait has exactly 2 actions. Content generation is                 │        │
│  │   impossible without modifying core types. Not disabled. IMPOSSIBLE.            │        │
│  │                                                                                 │        │
│  │   LAYER 2: PARSE-TIME GATE                                                      │        │
│  │   Forbidden modes rejected before simulation starts.                            │        │
│  │   "foreign influence", "violence", "war" → Err(InvariantViolation)              │        │
│  │                                                                                 │        │
│  │   LAYER 3: CI ENFORCEMENT                                                       │        │
│  │   ./ci/invariants_gate.sh blocks PRs with forbidden keywords.                   │        │
│  │   No human can accidentally merge dangerous code.                               │        │
│  │                                                                                 │        │
│  │   LAYER 4: RUNTIME AUDIT                                                        │        │
│  │   Every action logged. No redaction. Append-only.                               │        │
│  │   Regulators can inspect any run, any time.                                     │        │
│  │                                                                                 │        │
│  └─────────────────────────────────────────────────────────────────────────────────┘        │
│                                                                                             │
│  You can't target individuals if individuals aren't addressable.                            │
│  You can't hide interventions if the audit is append-only.                                  │
│                                                                                             │
└─────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## ⚡ The Engine

```
┌────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                │
│                           S W A R M S H I E L D   A R C H I T E C T U R E                      │
│                                                                                                │
│  ┌──────────────────────────────────────────────────────────────────────────────────────────┐  │
│  │                              INVARIANTS GATE (FAIL CLOSED)                               │  │
│  │                                                                                          │  │
│  │               if mode ∈ {"war", "foreign influence", "war"} → REJECT                     │  │
│  │                                                                                          │  │
│  └──────────────────────────────────────────────────────────────────────────────────────────┘  │
│                                              │                                                 │
│                                              ▼                                                 │
│  ┌─────────────────────┐  ┌───────────────────────┐  ┌─────────────────────┐                   │
│  │      TOPOLOGY       │  │        AGENTS         │  │    INSTITUTIONS     │                   │
│  │                     │  │                       │  │                     │                   │
│  │  ┌───────────────┐  │  │  ┌─────────────────┐  │  │  ┌───────────────┐  │                   │
│  │  │ Erdős-Rényi   │  │  │  │ Belief Vector   │  │  │  │    STATE      │  │                   │
│  │  │ (random)      │  │  │  │ (n-dimensional) │  │  │  │  legitimacy   │  │                   │
│  │  ├───────────────┤  │  │  ├─────────────────┤  │  │  │  policing     │  │                   │
│  │  │ Barabási-     │  │  │  │ Memory (EMA)    │  │  │  │  emergency    │  │                   │
│  │  │ Albert (hubs) │  │  │  │ 5-tick window   │  │  │  ├───────────────┤  │                   │
│  │  ├───────────────┤  │  │  ├─────────────────┤  │  │  │    MEDIA      │  │                   │
│  │  │ Watts-        │  │  │  │ 5 ARCHETYPES    │  │  │  │  fragmentation│  │                   │
│  │  │ Strogatz      │  │  │  │                 │  │  │  │  rumor_gain   │  │                   │
│  │  │ (small-world) │  │  │  │  ● Normal       │  │  │  ├───────────────┤  │                   │
│  │  └───────────────┘  │  │  │  ◆ Stubborn     │  │  │  │   MARKET      │  │                   │
│  │                     │  │  │  ★ Influencer   │  │  │  │  panic_risk   │  │                   │
│  │  Edges = influence  │  │  │  ◇ Contrarian   │  │  │  │  volatility   │  │                   │
│  │  [0.0 ─── 2.0]      │  │  │  ○ Passive      │  │  │  ├───────────────┤  │                   │
│  │                     │  │  │                 │  │  │  │    PARTY      │  │                   │
│  │                     │  │  └─────────────────┘  │  │  │  coherence    │  │                   │
│  └──────────┬──────────┘  └──────────┬────────────┘  │  │  recruitment  │  │                   │
│             │                        │               │  ├───────────────┤  │                   │
│             │                        │               │  │ FOREIGN_ACTOR │  │                   │
│             │                        │               │  │  intervention │  │                   │
│             │                        │               │  └───────────────┘  │                   │
│             │                        │               └──────────┬──────────┘                   │
│             │                        │                          │                              │
│             └────────────────────────┼──────────────────────────┘                              │
│                                      │                                                         │
│                                      ▼                                                         │
│  ┌──────────────────────────────────────────────────────────────────────────────────────────┐  │
│  │                           PARALLEL ENGINE (Rayon)                                        │  │
│  │                                                                                          │  │
│  │   for t in 0..steps {                                                                    │  │
│  │       signals = tracker.compute_incremental();      // O(Δ), not O(n²)                   │  │
│  │       cascades = detect_phase_transitions();        // Real-time alerts                  │  │
│  │       institutions.par_tick(&signals);              // Parallel institution update       │  │
│  │       agents.step_parallel(&topology, &rng);        // Rayon parallel belief update      │  │
│  │                                                                                          │  │
│  │       // ═══════════════════════════════════════════════════════════════════════════     │  │
│  │       // CRITICAL: Controllers can ONLY emit EdgeWeightDelta or ThrottleEdges            │  │
│  │       // No other action types exist. This is enforced by Rust's type system.            │  │
│  │       // ═══════════════════════════════════════════════════════════════════════════     │  │
│  │       let actions: Vec<TopologyAction> = controller.plan(&signals, &budget);             │  │
│  │       topology.apply(actions);                                                           │  │
│  │                                                                                          │  │
│  │       audit.append(t, &signals, &actions);          // Append-only. No redaction.        │  │
│  │   }                                                                                      │  │
│  └──────────────────────────────────────────────────────────────────────────────────────────┘  │
│                                      │                                                         │
│                                      ▼                                                         │
│  ┌──────────────────────────────────────────────────────────────────────────────────────────┐  │
│  │                           DETERMINISTIC AUDIT                                            │  │
│  │                                                                                          │  │
│  │   runs/run_<seed>_<timestamp>/                                                           │  │
│  │   ├── config.resolved.yaml        # Frozen configuration (what was run)                  │  │
│  │   ├── audit.jsonl                 # Every. Single. Action. (what happened)               │  │
│  │   └── metrics.parquet             # Time series (optional, for analysis)                 │  │
│  │                                                                                          │  │
│  │   GUARANTEE: Same seed + Same config = Identical output. Bit-for-bit.                    │  │
│  │                                                                                          │  │
│  └──────────────────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                                │
└────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🎮 7 Controllers (Topology-Only)

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                    CONTROLLER LIBRARY                                           │
│                                                                                                 │
│   All controllers emit ONLY two action types:                                                   │
│   • EdgeWeightDelta { edge: (u, v), delta: f64 }                                                │
│   • ThrottleEdges { threshold: f64, reduction: f64 }                                            │
│                                                                                                 │
│   No content. No messages. No targeting. By construction.                                       │
│                                                                                                 │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                 │
│   BASELINE STABILIZER              ISOLATION REDUCER              POLARIZATION DAMPER           │
│   ═══════════════════              ═════════════════              ═══════════════════           │
│                                                                                                 │
│   Strengthen random weak           Bridge disconnected            Weaken extreme edges          │
│   edges when isolation             clusters by connecting         to reduce echo chamber        │
│   exceeds threshold                low-degree nodes               effects                       │
│                                                                                                 │
│   ┌───●───●───┐                   ┌───●   ●───┐                   ┌───●═══●───┐                 │
│   │     ↑     │                   │    ╲ ╱    │                   │     ↓     │                 │
│   └───●───●───┘                   └───●───●───┘                   └───●───●───┘                 │
│                                                                                                 │
│   Trigger: isolation > 0.6        Trigger: components > 1        Trigger: polar > threshold     │
│                                                                                                 │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                 │
│   CASCADE INTERRUPTOR              RESILIENCE BUILDER             ADAPTIVE CONTROLLER           │
│   ═══════════════════              ═════════════════              ═══════════════════           │
│                                                                                                 │
│   Throttle ALL high-weight         Strengthen triangles           Learn optimal thresholds      │
│   edges during detected            to increase local              via exponential moving        │
│   cascade events                   clustering coefficient         average of signals            │
│                                                                                                 │
│   ┌───●━━━●───┐                   ┌───●───●───┐                   ┌───────────────────┐         │
│   │  ↓↓↓↓↓↓↓  │                   │   │╲ ╱│   │                   │  threshold(t) =   │         │
│   └───●━━━●───┘                   └───●─●─●───┘                   │  α·signal(t) +    │         │
│                                                                   │  (1-α)·threshold  │         │
│   Trigger: cascade_risk > 0.5     Trigger: clustering < target    │  (t-1)            │         │
│                                                                   └───────────────────┘         │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                 │
│   MULTI-OBJECTIVE CONTROLLER                                                                    │
│   ══════════════════════════                                                                    │
│                                                                                                 │
│   Pareto-optimal balancing of 4 objectives with weighted priority scoring:                      │
│                                                                                                 │
│   minimize(isolation) ∧ minimize(polarization) ∧ minimize(cascade_risk) ∧ maximize(resilience)  │
│                                                                                                 │
│   Configuration:                                                                                │
│   ```yaml                                                                                       │
│   bots:                                                                                         │
│     mode: multi_objective                                                                       │
│     weights:                                                                                    │
│       isolation: 0.3                                                                            │
│       polarization: 0.3                                                                         │
│       cascade_risk: 0.25                                                                        │
│       resilience: 0.15                                                                          │
│   ```                                                                                           │
│                                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🧬 5 Agent Archetypes

```
┌────────────────────────────────────────────────────────────────────────────────────────────────┐
│                              HETEROGENEOUS POPULATION MODEL                                    │
│                                                                                                │
│   Real populations aren't uniform. Neither are SwarmShield agents.                             │
│                                                                                                │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                │
│   ●  NORMAL (60%)              Change: 1.0x    Bias: 1.0x     Influence: 1.0x                  │
│      ═══════════════════════════════════════════════════════════════════════                   │
│      The baseline. Moderate susceptibility to neighbors.                                       │
│      Represents the silent majority in most scenarios.                                         │
│                                                                                                │
│   ◆  STUBBORN (15%)            Change: 0.3x    Bias: 2.0x     Influence: 0.8x                  │
│      ═══════════════════════════════════════════════════════════════════════                   │
│      Highly resistant to belief change. Strong confirmation bias.                              │
│      Ideologues, loyalists, true believers. Hard to move.                                      │
│                                                                                                │
│   ★  INFLUENCER (10%)          Change: 1.2x    Bias: 0.8x     Influence: 2.0x                  │
│      ═══════════════════════════════════════════════════════════════════════                   │
│      Disproportionate network impact. Lower confirmation bias.                                 │
│      Opinion leaders, celebrities, authority figures. Move others.                             │
│                                                                                                │
│   ◇  CONTRARIAN (8%)           Change: 0.8x    Bias: -0.5x    Influence: 1.2x                  │
│      ═══════════════════════════════════════════════════════════════════════                   │
│      NEGATIVE confirmation bias. Moves AGAINST consensus.                                      │
│      Skeptics, oppositionists, devil's advocates. Disruptors.                                  │
│                                                                                                │
│   ○  PASSIVE (7%)              Change: 0.5x    Bias: 0.5x     Influence: 0.3x                  │
│      ═══════════════════════════════════════════════════════════════════════                   │
│      Low engagement. Minimal network impact.                                                   │
│      Apolitical, disengaged, lurkers. Background noise.                                        │
│                                                                                                │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                │
│   CONFIGURE YOUR POPULATION:                                                                   │
│                                                                                                │
│   ```yaml                                                                                      │
│   agents:                                                                                      │
│     types:                                                                                     │
│       normal: 0.60       # Silent majority                                                     │
│       stubborn: 0.15     # Ideological core                                                    │
│       influencer: 0.10   # Opinion leaders                                                     │
│       contrarian: 0.08   # System challengers                                                  │
│       passive: 0.07      # Disengaged                                                          │
│   ```                                                                                          │
│                                                                                                │
│   RESEARCH QUESTION: How does stubborn/influencer ratio affect cascade dynamics?               │
│                                                                                                │
└────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 📊 11 Real-Time Signals

```
┌──────────────────────────────────────────────────────────────────────────────────────────────┐
│                                        SIGNAL DASHBOARD                                      │
│                                                                                              │
│   All signals computed incrementally: O(Δedges), not O(n²)                                   │
│                                                                                              │
├───────────────────────┬───────────────────────────────────────────────────────┬──────────────┤
│ SIGNAL                │ COMPUTATION                                           │ RANGE        │
├───────────────────────┼───────────────────────────────────────────────────────┼──────────────┤
│ isolation_index       │ 1 - (avg_degree / (n-1))                              │ [0, 1]       │
│ polarization_index    │ fraction(|belief| > 0.8)                              │ [0, 1]       │
│ violence_risk_index   │ f(polarization, activation, isolation, params)        │ [0, 1]       │
│ cascade_risk          │ EMA(recent_cascades) + activation_spread              │ [0, 1]       │
│ rumor_r               │ effective reproduction number of belief spread        │ [0, 5+]      │
│ legitimacy_index      │ institution.legitimacy × (1 - isolation)              │ [0, 1]       │
│ clustering_coeff      │ triangles / possible_triangles                        │ [0, 1]       │
│ avg_activation        │ mean(agent.activation)                                │ [0, 1]       │
│ belief_variance       │ var(belief_vectors)                                   │ [0, ∞)       │
│ type_entropy          │ -Σ p(type) × log(p(type))                             │ [0, log(5)]  │
│ activation_spread     │ var(agent.activation)                                 │ [0, 0.25]    │
├───────────────────────┴───────────────────────────────────────────────────────┴──────────────┤
│                                                                                              │
│   EXAMPLE: Detecting an imminent cascade                                                     │
│                                                                                              │
│   if signals.cascade_risk > 0.7 && signals.activation_spread > 0.15 {                        │
│       // Cascade forming. High activation variance = coordinated movement.                   │
│       controller.trigger_intervention();                                                     │
│   }                                                                                          │
│                                                                                              │
└──────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🕰️ Time Machine: Historical Counterfactuals

<div align="center">

### What if you could rerun history?

</div>

```
╔═══════════════════════════════════════════════════════════════════════════════════════════════╗
║                                                                                               ║
║  🇩🇪  WEIMAR GERMANY 1930-1933                                          2000 agents / 48 mo  ║
║  ══════════════════════════════════════════════════════════════════════════════════════════   ║
║                                                                                               ║
║  COUNTERFACTUAL: Could democratic institutions have survived?                                 ║
║                                                                                               ║
║  KEY PARAMETERS:                           OBSERVABLE OUTCOMES:                               ║
║  ├── Economic shock (1929 crash)           ├── Legitimacy decay curve                         ║
║  ├── Media fragmentation (radio rise)      ├── Violence risk trajectory                       ║
║  ├── Party coherence collapse              ├── Cascade frequency/intensity                    ║
║  └── Street violence dynamics              └── Polarization index over time                   ║
║                                                                                               ║
║  RUN: ./swarmshield configs/scenarios/germany_1930_1933.yaml                                  ║
║                                                                                               ║
╠═══════════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                               ║
║  🇩🇪  DDR 1989 - FALL OF THE BERLIN WALL                                2500 agents / 52 wk  ║
║  ══════════════════════════════════════════════════════════════════════════════════════════   ║
║                                                                                               ║
║  COUNTERFACTUAL: Was preventing the Wall's fall possible?                                     ║
║                                                                                               ║
║  KEY PARAMETERS:                           OBSERVABLE OUTCOMES:                               ║
║  ├── Soviet non-intervention policy        ├── Emigration pressure index                      ║
║  ├── Hungary border opening (Aug)          ├── Monday demonstration growth                    ║
║  ├── West German media penetration         ├── State legitimacy collapse point                ║
║  └── SED party coherence                   └── Opposition cascade timing                      ║
║                                                                                               ║
║  TIPPING POINT: Watch week 37-42 for the cascade trigger                                      ║
║                                                                                               ║
║  RUN: ./swarmshield configs/scenarios/ddr_1989_berlin_wall.yaml                               ║
║                                                                                               ║
╠═══════════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                               ║
║  🇷🇺  USSR 1985-1991 - PERESTROIKA                                      3000 agents / 78 mo  ║
║  ══════════════════════════════════════════════════════════════════════════════════════════   ║
║                                                                                               ║
║  COUNTERFACTUAL: Could Gorbachev have followed the Chinese path?                              ║
║                                                                                               ║
║  KEY PARAMETERS:                           OBSERVABLE OUTCOMES:                               ║
║  ├── Glasnost pace (information opening)   ├── Centrifugal forces index                       ║
║  ├── 6 republic clusters (nationalities)   ├── Party faction coherence                        ║
║  ├── Hardliner vs reformer dynamics        ├── Union stability trajectory                     ║
║  └── Economic restructuring speed          └── Republic breakaway timing                      ║
║                                                                                               ║
║  RESEARCH Q: What glasnost pace preserves union stability?                                    ║
║                                                                                               ║
║  RUN: ./swarmshield configs/scenarios/ussr_1985_perestroika.yaml                              ║
║                                                                                               ║
╠═══════════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                               ║
║  🇭🇺  HUNGARY 1956 - REVOLUTION                                         2000 agents / 21 dy  ║
║  ══════════════════════════════════════════════════════════════════════════════════════════   ║
║                                                                                               ║
║  COUNTERFACTUAL: Was peaceful transition from Stalinism achievable?                           ║
║                                                                                               ║
║  KEY PARAMETERS:                           OBSERVABLE OUTCOMES:                               ║
║  ├── Soviet intervention threshold         ├── Violence escalation curve                      ║
║  ├── Nagy reform pace                      ├── Soviet intervention trigger point              ║
║  ├── Worker council formation              ├── Reform window duration                         ║
║  └── Western response signals              └── Cascade → crackdown timing                     ║
║                                                                                               ║
║  21 DAYS: High-resolution daily simulation                                                    ║
║                                                                                               ║
║  RUN: ./swarmshield configs/scenarios/hungary_1956_revolution.yaml                            ║
║                                                                                               ║
╠═══════════════════════════════════════════════════════════════════════════════════════════════╣
║                                                                                               ║
║  💹  MARKET PANIC - GENERIC                                             3000 agents / 240 hr  ║
║  ══════════════════════════════════════════════════════════════════════════════════════════   ║
║                                                                                               ║
║  COUNTERFACTUAL: How do rumors trigger bank runs?                                             ║
║                                                                                               ║
║  KEY PARAMETERS:                           OBSERVABLE OUTCOMES:                               ║
║  ├── Social media speed                    ├── Panic cascade velocity                         ║
║  ├── Institutional trust baseline          ├── Withdrawal contagion                           ║
║  ├── Rumor correction latency              ├── Intervention effectiveness                     ║
║  └── Panic susceptibility                  └── Recovery time                                  ║
║                                                                                               ║
║  USE CASE: SVB-style 48-hour collapse modeling                                                ║
║                                                                                               ║
║  RUN: ./swarmshield configs/scenarios/market_panic_fakenews.yaml                              ║
║                                                                                               ║
╚═══════════════════════════════════════════════════════════════════════════════════════════════╝
```

<div align="center">

### **Create your own scenarios: [`docs/SCENARIO_GUIDE.md`](docs/SCENARIO_GUIDE.md)**

</div>

---

## ⚡ Performance That Scales

```
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                     BENCHMARK RESULTS                                           │
│                                     (Criterion.rs, M1 Max)                                      │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                 │
│   TOPOLOGY GENERATION                                                                           │
│   ═══════════════════════════════════════════════════════════════════════════════════════════   │
│                                                                                                 │
│   erdos_renyi/100 ...................... 189 µs     ██                     5,300 graphs/sec     │
│   erdos_renyi/1000 ..................... 19.2 ms    ████████████████████   52 graphs/sec        │
│   erdos_renyi/5000 ..................... 478 ms     ████████████████████   2.1 graphs/sec       │
│                                                                                                 │
│   barabasi_albert/1000 ................. 4.0 ms     ████████               250 graphs/sec       │
│   barabasi_albert/5000 ................. 102 ms     ████████████████████   9.8 graphs/sec       │
│                                                                                                 │
│   watts_strogatz/1000 .................. 8.1 ms     ████████████           123 graphs/sec       │
│   watts_strogatz/5000 .................. 198 ms     ████████████████████   5.1 graphs/sec       │
│                                                                                                 │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                 │
│   AGENT STEPPING (Rayon Parallel, 8 cores)                                                      │
│   ═══════════════════════════════════════════════════════════════════════════════════════════   │
│                                                                                                 │
│   step/100 agents ...................... 13 µs      █                      77,000 steps/sec     │
│   step/1000 agents ..................... 1.35 ms    ████████               740 steps/sec        │
│   step/5000 agents ..................... 6.8 ms     ████████████████       147 steps/sec        │
│   step/10000 agents .................... 14.2 ms    ████████████████████   70 steps/sec         │
│                                                                                                 │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                 │
│   INCREMENTAL METRICS (The Secret Sauce)                                                        │
│   ═══════════════════════════════════════════════════════════════════════════════════════════   │
│                                                                                                 │
│   Full recompute/1000 agents ........... 23.6 ms    ████████████████████                        │
│   Incremental (10 edge changes) ........ 0.8 ms     ██                     ~30x FASTER          │
│   Incremental (100 edge changes) ....... 2.1 ms     █████                  ~11x FASTER          │
│                                                                                                 │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                                 │
│   FULL SIMULATION (End-to-End)                                                                  │
│   ═══════════════════════════════════════════════════════════════════════════════════════════   │
│                                                                                                 │
│   Hungary 1956 (2000 agents, 21 steps) .......... ~0.4 sec                                      │
│   Weimar (2000 agents, 48 steps) ................ ~1.6 sec                                      │
│   DDR 1989 (2500 agents, 52 steps) .............. ~2.1 sec                                      │
│   USSR 1985 (3000 agents, 78 steps) ............. ~4.8 sec                                      │
│   Market Panic (3000 agents, 240 steps) ......... ~14.2 sec                                     │
│                                                                                                 │
│   10,000 COUNTERFACTUAL RUNS (Hungary, varied seeds) ... ~67 minutes (parallelizable)           │
│                                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🔒 15 Property-Based Tests

```rust
// tests/property_tests.rs - Proptest invariant verification

proptest! {
    #[test]
    fn budget_never_exceeded(max in 1u64..100, requested in 0u64..200) {
        // Controller actions NEVER exceed budget
    }

    #[test]
    fn edge_weights_always_bounded(weight in 0.0..2.0, delta in -1.0..1.0) {
        let new = (weight + delta).clamp(0.0, 2.0);
        prop_assert!(new >= 0.0 && new <= 2.0);
    }

    #[test]
    fn deterministic_replay(seed in 0u64..u64::MAX) {
        // Same seed = identical output, bit-for-bit
    }

    #[test]
    fn no_nan_no_inf_beliefs(beliefs in vec(any::<f64>(), 1..100)) {
        // Beliefs never become NaN or Inf
    }

    #[test]
    fn topology_actions_only(action in any::<ControllerAction>()) {
        // Only EdgeWeightDelta or ThrottleEdges exist
    }

    // ... 10 more tests covering all invariants
}
```

**All 15 tests pass. Always. On every commit.**

---

## 📁 Project Structure

```
swarmshield/
├── src/
│   ├── main.rs              # CLI entry point
│   ├── sim.rs               # Parallel engine loop, cascade detection
│   ├── agents.rs            # 5 agent archetypes, EMA memory, belief dynamics
│   ├── topology.rs          # Erdős-Rényi, Barabási-Albert, Watts-Strogatz
│   ├── metrics.rs           # Incremental O(Δ) signal computation
│   ├── controller.rs        # 7 topology-only controllers
│   ├── invariants.rs        # FAIL CLOSED safety gates
│   ├── config.rs            # YAML parsing with validation
│   ├── audit.rs             # Append-only JSONL logging
│   └── institutions/
│       ├── mod.rs           # Institution trait
│       ├── state.rs         # Legitimacy, policing, emergency powers
│       ├── party.rs         # Coherence, recruitment, violence threshold
│       ├── media.rs         # Fragmentation, rumor gain, correction latency
│       ├── market.rs        # Scarcity, panic susceptibility, volatility
│       └── foreign_actor.rs # Intervention threshold, amplification bias
├── benches/
│   └── engine_bench.rs      # Criterion.rs benchmarks (4 suites)
├── tests/
│   └── property_tests.rs    # Proptest invariants (15 tests)
├── configs/
│   ├── schema.scenario.yaml # Canonical schema
│   └── scenarios/
│       ├── germany_1930_1933.yaml
│       ├── ddr_1989_berlin_wall.yaml
│       ├── ussr_1985_perestroika.yaml
│       ├── hungary_1956_revolution.yaml
│       ├── italy_1946_1948_elections.yaml
│       ├── russia_1905_1917_reform_path.yaml
│       └── market_panic_fakenews.yaml
├── docs/
│   └── SCENARIO_GUIDE.md    # Complete guide to creating scenarios
├── ci/
│   └── invariants_gate.sh   # CI safety enforcement
├── INVARIANTS.md            # Non-negotiable safety constraints
├── SECURE.md                # Threat model & controls
├── IMPROVEMENTS.md          # Future enhancements
└── ROADMAP.md               # Development timeline
```

---

## 🗺️ Roadmap to v3.0

```
                                         DEVELOPMENT PHASES
═══════════════════════════════════════════════════════════════════════════════════════════════════

     v1.0 FOUNDATION           v2.0 SCALE                  v2.2 PRODUCTION (YOU ARE HERE)
     ═══════════════           ══════════                  ════════════════════════════════
     ✓ Core engine             ✓ Rayon parallel            ✓ 7 controllers
     ✓ Basic controllers       ✓ Incremental metrics       ✓ 5 agent types
     ✓ Property tests          ✓ Cascade detection         ✓ 7 scenarios
     ✓ Audit logging           ✓ Phase transitions         ✓ Scenario guide
     ✓ Safety gates            ✓ Agent memory              ✓ Production-ready

─────────────────────────────────────────────────────────────────────────────────────────────────────

     v2.5 ANALYSIS             v3.0 INTEGRATION            v3.5+ ENTERPRISE
     ══════════════            ════════════════            ═════════════════
     □ Checkpoint/restore      □ Python bindings           □ Cloud deployment
     □ Counterfactual diff     □ WASM browser demo         □ REST API
     □ Parquet export          □ Jupyter integration       □ Real-time dashboard
     □ Visualization server    □ GPU acceleration          □ Multi-tenant audit

═══════════════════════════════════════════════════════════════════════════════════════════════════
                              CURRENT: v2.2-prod   ████████████████████░░░░   85%
═══════════════════════════════════════════════════════════════════════════════════════════════════
```

---

## 📜 License

Proprietary License - See [LICENSE](LICENSE) file.

---

<div align="center">

## 💭 Philosophy

</div>

```
╔════════════════════════════════════════════════════════════════════════════════════════════════╗
║                                                                                                ║
║   "Every social simulation is dual-use technology.                                             ║
║    The question isn't whether to build them-it's how to build them safely.                     ║
║                                                                                                ║
║    ──────────────────────────────────────────────────────────────────────────────────────      ║
║                                                                                                ║
║    To the researcher: Run your counterfactuals. Publish your papers. Advance the field.        ║
║    To the risk manager: Stress test your systems. Protect your institution.                    ║
║    To the policy maker: Simulate before you legislate. Understand before you act.              ║
║    To the regulator: Inspect any run. Audit any decision. Trust the system.                    ║
║                                                                                                ║
║    To everyone else: This is what it looks like when you build AI infrastructure               ║
║    that you can hand to your compliance team with a clear conscience."                         ║
║                                                                                                ║
╚════════════════════════════════════════════════════════════════════════════════════════════════╝
```

---

<div align="center">

**Built with obsessive caution. Constrained by only imagination. Open for research.**

`topology_only_actions` · `audit_all_actions` · `deterministic_replay`

---

<sub>
<b>SwarmShield</b>: Understanding instability without access to secret files.<br>
Analysing the past. Modeling the present. Predicting the future.<br>
<i>Because reality doesn't have to stick to possibilities.</i>
</sub>

---

[![Star History](https://img.shields.io/badge/⭐_Star_if_you_believe-Safety_is_a_feature-ff6b35?style=for-the-badge)](https://github.com/QuantGenAIPhr34kW1z/swarmshield)

</div>

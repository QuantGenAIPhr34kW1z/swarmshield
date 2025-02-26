# Scenario Creation Guide

This guide explains how to create new SwarmShield scenarios for counterfactual analysis of social dynamics.

---

## Table of Contents

1. [Philosophy](#philosophy)
2. [Scenario Structure](#scenario-structure)
3. [Design Process](#design-process)
4. [Parameter Reference](#parameter-reference)
5. [Examples by Domain](#examples-by-domain)
6. [Validation Checklist](#validation-checklist)
7. [Common Patterns](#common-patterns)

---

## Philosophy

SwarmShield scenarios are **research tools**, not prediction engines. They help answer questions like:

- "What conditions would have been necessary for X to happen?"
- "How sensitive was outcome Y to parameter Z?"
- "What intervention strategies could have changed trajectory T?"

**Critical constraints** (see `INVARIANTS.md`):
- No content generation or message creation
- No individual targeting
- Topology-only interventions
- Full audit trail

---

## Scenario Structure

Every scenario is a YAML file with these sections:

```yaml
version: "0.1"
seed: <integer>           # Deterministic reproducibility

world:
  dt: <float>             # Time step (usually 1.0)
  steps: <integer>        # Number of simulation steps
  parallel: <bool>        # Enable parallel processing
  topology: { ... }       # Network structure

agents:
  n: <integer>            # Number of agents
  state_model: { ... }    # Belief dimensions and initialization
  dynamics: { ... }       # Behavioral parameters
  types: { ... }          # Agent type distribution

institutions:
  - id: <string>
    kind: <type>
    params: { ... }

bots:
  enabled: <bool>
  mode: <controller>
  budget: { ... }

metrics:
  track: [...]            # Metrics to log

rules:
  invariants: [...]       # Safety constraints
```

---

## Design Process

### Step 1: Define the Counterfactual Question

Start with a clear research question:

```
GOOD: "Could the Berlin Wall have remained standing with different Soviet policy?"
BAD:  "Simulate Germany 1989"
```

The question should:
- Be falsifiable through simulation
- Have clear success/failure metrics
- Not require content generation

### Step 2: Identify Key Actors

Map real-world actors to institutions:

| Real World | SwarmShield | Example |
|------------|-------------|---------|
| Government | `state` | Legitimacy, policing |
| Media outlets | `media` | Fragmentation, rumor gain |
| Political parties | `party` | Coherence, recruitment |
| Economy | `market` | Scarcity, volatility |
| External powers | `foreign_actor` | Intervention threshold |

### Step 3: Design Belief Dimensions

Choose 3-5 belief dimensions that capture key attitudes:

```yaml
# Example: Cold War scenario
# Dimension 0: Trust in state (negative = distrust)
# Dimension 1: Desire for change (positive = revolutionary)
# Dimension 2: Economic grievance (positive = dissatisfied)
# Dimension 3: Fear of repression (positive = afraid)
```

**Guidelines:**
- Use symmetric scales centered around 0
- Make dimensions orthogonal (not redundant)
- Document what each dimension means

### Step 4: Set Initial Conditions

Use clusters for heterogeneous populations:

```yaml
agents:
  state_model:
    init:
      kind: clusters
      clusters:
        k: 5      # Number of distinct groups
        spread: 0.8  # Within-group variance
```

**k (cluster count)** examples:
- `k=2`: Binary division (pro/anti)
- `k=3`: Spectrum (left/center/right)
- `k=5`: Complex society (multiple factions)

### Step 5: Calibrate Dynamics

| Parameter | Low | Medium | High | Effect |
|-----------|-----|--------|------|--------|
| `reinforcement` | 0.01 | 0.03 | 0.06 | Echo chamber strength |
| `decay` | 0.005 | 0.01 | 0.02 | Belief regression to mean |
| `noise` | 0.01 | 0.02 | 0.04 | Random fluctuation |
| `confirmation_bias` | 0.03 | 0.05 | 0.08 | In-group preference |
| `isolation_sensitivity` | 0.04 | 0.07 | 0.10 | Radicalization of isolated |
| `violence_risk_gain` | 0.01 | 0.025 | 0.05 | Violence probability |

### Step 6: Configure Institutions

#### State
```yaml
- id: "example_state"
  kind: state
  params:
    legitimacy: 0.50        # [0,1] Initial legitimacy
    policing_friction: 0.25 # [0,1] Repression capability
    emergency_powers: 0.30  # [0,1] Crisis response capacity
    trust_floor: 0.15       # [0,1] Minimum achievable trust
```

#### Media
```yaml
- id: "example_media"
  kind: media
  params:
    fragmentation: 0.60     # [0,1] Source diversity
    amplification_volatility: 0.40  # [0,1] News cycle speed
    rumor_gain: 0.30        # [0,1] Misinformation spread
    correction_latency: 0.50  # [0,1] Fact-check delay
```

#### Market
```yaml
- id: "example_market"
  kind: market
  params:
    scarcity_index: 0.45    # [0,1] Resource scarcity
    unemployment_pressure: 0.30  # [0,1] Job insecurity
    volatility: 0.40        # [0,1] Price instability
    panic_susceptibility: 0.35  # [0,1] Bank run likelihood
```

#### Party
```yaml
- id: "example_party"
  kind: party
  params:
    coherence_strength: 0.55  # [0,1] Internal unity
    recruitment_rate: 0.04    # [0,1] Growth rate
    propaganda_budget: 0.40   # [0,1] Messaging capacity
    legitimacy_pull: 0.50     # [0,1] Popular appeal
    violence_threshold: 0.30  # [0,1] When force is used
```

#### Foreign Actor
```yaml
- id: "example_foreign"
  kind: foreign_actor
  params:
    intervention_threshold: 0.70  # [0,1] When they intervene
    amplification_bias: 0.20      # [-1,1] Pro (+) or anti (-) reform
    destabilization_rate: 0.15    # [0,1] Active interference
    disinformation_level: 0.20    # [0,1] Fake news injection
```

### Step 7: Choose Controller

| Controller | Best For |
|------------|----------|
| `baseline` | Simple isolation reduction |
| `adaptive` | Learning optimal thresholds |
| `multi_objective` | Balancing multiple goals |
| `cascade_interruptor` | Preventing viral spread |
| `polarization_damper` | Reducing extremism |

### Step 8: Define Success Metrics

Document what "success" means for your counterfactual:

```yaml
# In scenario comments:
# Success metrics for "peaceful transition":
# - legitimacy_index > 0.40 at end
# - violence_risk_index < 0.30 throughout
# - polarization_index < 0.50
# - No cascade events > 10% of population
```

---

## Parameter Reference

### Topology Generators

| Generator | Parameters | Best For |
|-----------|------------|----------|
| `erdos_renyi` | `n`, `p` | Random networks |
| `barabasi_albert` | `n`, `m` | Scale-free (influencers) |
| `watts_strogatz` | `n`, `k`, `beta` | Small-world communities |

### Agent Types

| Type | Change Rate | Confirmation Bias | Influence | Use For |
|------|-------------|-------------------|-----------|---------|
| `normal` | 1.0x | 1.0x | 1.0x | General population |
| `stubborn` | 0.3x | 2.0x | 0.8x | Ideologues, loyalists |
| `influencer` | 1.2x | 0.8x | 2.0x | Leaders, celebrities |
| `contrarian` | 0.8x | -0.5x | 1.2x | Skeptics, oppositionists |
| `passive` | 0.5x | 0.5x | 0.3x | Apolitical citizens |

---

## Examples by Domain

### Historical Counterfactuals

```
Question: "What if X had happened differently?"
Focus: Path dependence, tipping points
Key: Identify critical decision points
Example: germany_1930_1933.yaml
```

### Market Dynamics

```
Question: "What causes financial panics?"
Focus: Information cascades, herding
Key: High panic_susceptibility, volatile media
Example: market_panic_fakenews.yaml
```

### Political Transitions

```
Question: "When do revolutions succeed/fail?"
Focus: Legitimacy erosion, violence thresholds
Key: State legitimacy, foreign intervention
Example: hungary_1956_revolution.yaml
```

### Institutional Collapse

```
Question: "What causes state failure?"
Focus: Compound crises, feedback loops
Key: Multiple institutions in crisis
Example: ussr_1985_perestroika.yaml
```

---

## Validation Checklist

Before running a scenario, verify:

### Structural Validity
- [ ] All required fields present
- [ ] Parameter values in valid ranges
- [ ] Agent count matches topology size
- [ ] Belief dimensions consistent

### Research Validity
- [ ] Counterfactual question clearly stated
- [ ] Success/failure metrics defined
- [ ] Historical context documented
- [ ] Intervention hypotheses listed

### Safety Compliance
- [ ] `no_persuasion` invariant included
- [ ] `topology_only_actions` invariant included
- [ ] `audit_all_actions` invariant included
- [ ] No individual targeting mechanisms

### Reproducibility
- [ ] Seed is meaningful date/number
- [ ] All parameters documented
- [ ] Expected behavior described

---

## Common Patterns

### Rapid Collapse Scenario

```yaml
agents:
  dynamics:
    reinforcement: 0.05      # High
    isolation_sensitivity: 0.09
    violence_risk_gain: 0.04
institutions:
  - kind: state
    params:
      legitimacy: 0.30       # Low
      trust_floor: 0.10
```

### Stable Equilibrium Scenario

```yaml
agents:
  dynamics:
    reinforcement: 0.02      # Low
    decay: 0.015             # High
    noise: 0.01              # Low
institutions:
  - kind: state
    params:
      legitimacy: 0.65       # High
```

### Information Cascade Scenario

```yaml
agents:
  dynamics:
    noise: 0.04              # High
institutions:
  - kind: media
    params:
      fragmentation: 0.80    # High
      rumor_gain: 0.50       # High
```

### Ethnic Conflict Scenario

```yaml
agents:
  state_model:
    init:
      kind: clusters
      clusters:
        k: 3                 # Ethnic groups
        spread: 0.5          # Low variance within groups
  dynamics:
    confirmation_bias: 0.08  # High
  types:
    stubborn: 0.25           # Many hardliners
```

---

## Running Your Scenario

```bash
# Build release version
cargo build --release

# Run scenario
./target/release/swarmshield configs/scenarios/your_scenario.yaml

# Output location
ls runs/run_<seed>_<timestamp>/
# → config.resolved.yaml
# → audit.jsonl

# Analyze results
# (See IMPROVEMENTS.md for planned analysis tools)
```

---

## Further Reading

- `INVARIANTS.md` - Safety constraints
- `README.md` - Architecture overview
- `IMPROVEMENTS.md` - Planned features
- `ROADMAP.md` - Development timeline

---

## Contributing Scenarios

1. Follow this guide
2. Include comprehensive comments
3. Document research question clearly
4. Submit PR with analysis notes
5. Scenarios must pass `./ci/invariants_gate.sh`

---

```
      ┌─────────────────────────────────────────────────────────────┐
      │                                                             │
      │   Good scenarios ask questions. They don't provide answers. │
      │                                                             │
      │   The simulation is a lens, not an oracle.                  │
      │                                                             │
      └─────────────────────────────────────────────────────────────┘
```

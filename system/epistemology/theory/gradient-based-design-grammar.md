# Gradient-Based Design Grammar (GBDG v0.1)

## 1. Motivating Intuition
⬡[PV0.1] 

Engineers rarely think in raw tensors. But their intent lives in gradients: desires, concerns, edge-cases.  
GBDG translates these into idiomatic expressions — small, collapsible intent structures — that preserve meaning and propagate accountability.

Why we need a grammar at all: expression ≠ projection, and without composable idioms, engineering intent stays mute.
## 2. Idiomatic Primitives

Smallest collapsible belief structures (e.g. “expected invariance,” “modular boundary,” “risky reuse”).

Each idiom encodes:
- A gradient shape in $\mathcal{F}$,
- A projection affordance,
- A trace function ($\tau_i$).

|Idiom|Gradient Interpretation|Example Intent|
|---|---|---|
|Invariance|Flat region, null $\nabla \Xi$ expected|“This must not change”|
|Boundary|Sharp $\Xi$ jump across $\Delta$|“These modules shouldn’t leak”|
|Volatility|Rapidly shifting $\Xi$, unstable $\tau_D$|“This is fragile under change”|
### 2.1 Distinguishing Idioms from Operators

An idiom is a *descriptive semantic configuration* — it expresses an intent, constraint, or expectation.  
An operator, by contrast, is an *active transformation* — it modifies the semantic field $\mathcal{F}$.

| Element     | Role                              | Executable? |
|-------------|-----------------------------------|-------------|
| Idiom       | Expresses intent as gradient form | No          |
| Operator    | Resolves or alters $\mathcal{F}$  | Yes         |

Idioms may be reified into operators during projection, but they themselves do not alter the field.  
Their purpose is expressive, not operational — to articulate what *kind* of collapse is intended, not how to perform it.

This separation allows:
- Expressive design without immediate execution,
- Deferred constraint resolution,
- Layered composability across semantic modules.

## 3. Intent Schema Layer

- Collocational schema for encoding: intent ↔ semantic gradient.
- Could be seed-compatible with existing TDD categories (e.g. precondition, invariant, contract breach, edge).

A structured idiom schema:
- Type: idiom (e.g., Invariance, Risk)
- Gradient target: where $\Delta$ is being applied
- Expected collapse: soft, deferred, immediate?
- Audit level: τ-minimal / τ+context / full

This could align to TDD-like tags:
- Precondition → Invariance idiom
- Contract → Boundary idiom
- Edge-case → Volatility idiom

### 3.1 Idiom Lifecycle and Persistence

Idioms behave like local semantic attractors in $\mathcal{F}$. If not projected, they:

- Remain as latent gradient structures,
- Drift via $\phi_{\text{pre}}$ contribution,
- Accumulate in scaffold zones ⬡[PV3.7],
- Or persist as rolling closures ⬡[PV6.11].

This means idioms can be:
- Collapsed: if they trigger $\mathcal{C}$,
- Deferred: stored in partial scaffolds,
- Persistent: as unresolved tensions awaiting future resolution.

Their persistence makes them useful even without immediate projection — they structure the field for future rhetorical or design navigation.

## 4. Composable Structures

How do multiple gradients become design surfaces or systems?  

Must define:
- Join-ability conditions (e.g. coherence across $\Xi$ gradients),
- Idiom tension alignment.

Semantic Join Conditions:
- Compatible $\phi_{\text{pre}}$ direction
- Non-conflicting $\nabla \Xi$ gradients
- Trace continuity rules

These allow higher-order constructs:
- _Design membrane_: region bounded by multiple idioms
- _Gradient cluster_: coherent $\Delta$ fields bundled under shared constraint

### 4.1 Minimal Join Conditions

To form valid idiom bundles, the following must hold:

- $\Delta_i, \Delta_j$ must be *coherently composable*, e.g., $\Delta_i + \Delta_j$ lies within smooth region of $\mathcal{F}$,
- $\nabla\Xi$ fields must be *non-destructively superposable*,
- Narrative trace continuity: $\tau_i \leadsto \tau_j$ (trace must be linkable).

We define a bundle $\mathcal{I}_k = \{ \iota_1, \iota_2, \dots \}$ as syntactically valid if all join conditions hold.

These bundles are candidates for:
- Design membranes (boundary-defined projection regions),
- Gradient clusters (semantically coherent bundles of idioms),
- Projection rehearsal in the scaffold layer.

Constraint satisfaction (⧉) may be applied *after* idioms have been joined, preserving expressibility before operational resolution.

### 5. Idiom Failure Modes

Even in a minimal expressibility system, idioms can fail — not by breaking code, but by failing to trigger meaningfully.

| Failure Mode       | Condition                                          | Result                                        |
|--------------------|---------------------------------------------------|-----------------------------------------------|
| Collapse-failure   | $\nabla_\Delta \Xi < \theta$                      | Intent never reaches belief                   |
| Projection-mismatch| Collapse occurs, but $\tau$ is unstable           | Volatile belief trace                         |
| Scaffold deferral  | Collapse condition unmet, $\iota \mapsto \mathcal{S}$ | Idiom floats in scaffold zone                 |
| Join conflict      | Bundle fails semantic compatibility tests         | Composition rejected or deferred              |

These failure types help:
- Debug failed or muted design efforts,
- Improve idiom bundling heuristics,
- Feed back into design intent refinement systems.

Over time, idiom failure analysis will support a lightweight *semantic linting engine* for pre-projection diagnostics.

## Integration Hints

How this grammar is likely to interface with:
- Constraint engine (future),
- $\mathcal{C}$ trace logic (now),
- UI design surface / dropdown exposure layers.

Likely surfaces:
- Middleware UI layer: idiom dropdowns, test declarations
- Projection module: evaluates idiom collapse thresholds
- Constraint engine (future): treats idioms as constraint priors


### 🧩 What’s Still Missing from GBDG Before It Can Be Built?

#### 1. Formal Idiom Table Schema

We still lack:
- A canonical set of idiom types
- Collapse behaviour flags (e.g. eager, deferred)
- Expressive role (assertive, neutral, boundary-making)
- Composability rules and rhetorical load
- Trace schema alignment (what part of $\tau$ it contributes to)    

_A structured idiom table would make the grammar auditable and interpretable by tools._

#### 2. Machine-Readable Representation of Idioms

We haven’t defined:
- A syntax or DSL for declaring idioms in source code or design UI
- A data model to represent idiom bundles in $\mathcal{F}$
- A link to test structures / expressions in TDD systems

This is needed for:
- Middleware integration
- Projection-triggering
- Constraint pre-processing

#### 3. Idiomatic Evaluation Layer

We have described idioms semantically, but not:
- How idiom bundles are evaluated for projection worthiness (prior to constraint solving)
- Whether they are traversed, prioritised, or buffered

Do they get “scanned” during build? Simulated during planning? Only surfaced during failures?

#### 4. Rhetorical Topology Support

Right now, idioms live in isolation. What’s missing:
- Mapping idioms to rhetorical priors ⬡[PV3.1]
- Enabling modulation (e.g. $\pi_{\text{sym}}$ acting on Boundary idioms)    
- Supporting affective idioms (Joy = cohesion? Irritation = threshold raise?)

This is key for reflexive design dynamics.

#### 5. Idiomatic Provenance and Audit Hooks

- Idioms must leave trace hooks in $\tau$
- But we haven’t defined if idioms leave pre-collapse traces
- We also don’t yet distinguish idiom _declaration_ from idiom _commitment_

This matters for time-travelling debug tools, rollback, and closure ecology.
## 6. Provocative Questions (v0.1-b)

1. Idiomatic Saturation – How large must the canonical idiom set be before additional idioms add more noise than expressive power?  
   _What objective metric (coverage ∕ redundancy) decides when the grammar is “complete”?_

2. DSL Minimality – What is the smallest machine-readable syntax that can encode an idiom bundle *and* its audit level without falling back to free-form prose?  
   _YAML fragments?  Rust macros?  A tiny lisp?_

3. Reification Threshold – At what field-pressure does an idiom graduate into an operator?  
   _Should the promotion rule be global (one θ) or idiom-specific?_

4. Neutral Idioms – Do non-rhetorical idioms (e.g. “junction”) serve any purpose other than bundling, or do they inevitably acquire a bias once composed?  
   _If they stay neutral, how are they visualised in $\tau$?_

5. Lifecycle Governance – Who (or what) decides when an idiom lingering in a scaffold zone must be pruned, promoted, or archived?  
   _Is time-to-live a system constant, or negotiated per project?_

6. Join-Conflict Diagnostics – If two idioms fail the minimal join test, should the grammar:  
   a) forbid the composition,  
   b) auto-scaffold them apart, or  
   c) mark a rhetorical dispute for human resolution?  

7. Trace Granularity – Does every idiom instance need its own $\tau_i$, or can closely related idioms share a composite trace node to limit audit bloat?

8. Affective Overlay – How is an idiom’s collapse probability altered if an affective prior (e.g. Joy or Irritation) modulates its region *after* declaration but *before* projection?

> _Answering even half of these questions is enough work for v0.2._

### 6.1 Extended Grammar Constraints (Under METED v0.1)

⬡[PV0.1], ⬡[PV1.1], ⬡[PV1.2], ⬡[PV1.3], ⬡[PV2.2], ⬡[PV2.3]

The following constraints derive directly from the *Minimal Expressibility Theory for Engineering Design (METED v0.1)* and delimit how far GBDG can go in its initial version:

- Only 5 core objects are permitted: $\mathcal{F}, \Xi, \Delta, \mathcal{C}, \tau_D$
- Only a single collapse rule may be applied:
  $$
  \left\lVert \nabla_{\!\! \Delta} \Xi \right\rVert > \theta_{\text{design}}
  $$
- Only a 3-tier trace schema is available, defined in terms of $\tau_D$ and its projected context.

These limitations imply the following:

- Idioms cannot introduce new operators. All semantic expressions must reduce to interpretable gradients in $\mathcal{F}$.
- No new projection types may be declared beyond $\mathcal{C} : (\mathcal{F}, \Delta) \to \mathcal{B}$.
- Trace expressions must resolve to $\tau_D$, or to simple linked extensions traceable through $\tau_D \leadsto \tau_i$ where $\tau_i \in \mathcal{B}$.

This means that even rich idioms, such as those involving rhetorical modulation or affective overlays, must defer their effects unless expressible directly via:

- Gradient sharpness or continuity in $\nabla_{\!\! \Delta} \Xi$
- Their proximity to a collapse event (in $\theta$-space)
- Or their coherence with an existing trace narrative

GBDG v0.1 is a semantic surface grammar — a pre-constraint idiom encoding mechanism — that prepares expressive bundles for future collapse and trace without exceeding METED’s minimal design boundary.

Subsequent versions (GBDG v0.2+) may reintroduce:

- Idiom-to-operator reification via rhetorical priors ⬡[PV3.1]
- Extended closure ecology ⬡[PV6.11]
- π-stack modulation ⬡[PV3.3] for resolving high-tension idioms

For now, idioms must live lightly: descriptive, composable, traceable — but not yet executable.
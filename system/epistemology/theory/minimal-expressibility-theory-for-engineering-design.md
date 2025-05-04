---
title: Minimal Expressibility Theory for Engineering Design (METED v0.1)
aliases:
  - Minimal Design-Expressibility Theory
  - METED
  - Rhetorical-Constraint Lite
status: draft-theory
version: "0.1"
created: 2025-05-04
updated: 2025-05-04
priority: high
author: Bee (+ conversational pruning)
project: semantic-agency-architecture
related:
  - "[[Minimal Theory for Belief Traceability (MTBT v0.1)]]"
  - "[[Constraint as Rhetoric — full]]"
summary: |-
  Provides the least theoretical machinery required for an engineering
  specification to be represented as semantic gradients and audited for
  coherence.  Retains only five formal objects, one collapse rule, and a
  three-tier trace scheme.  Everything else (π-stacks, TRL-inf, affect, etc.)
  is postponed to future passes.
pv_tags:
  - PV0.1
  - PV1.1
  - PV1.2
  - PV1.3
  - PV2.2
  - PV2.3
  - PV3.1
---
## 1. Motivating Engineering Intuition

⬡[PV0.1]

Good engineering designs *feel* coherent before they compile.  
Here “feeling” is formalised: a design is a gradient in meaning space.  
If a design cannot be smoothly continued without tearing the field, the gradient triggers collapse.

We want the smallest theory that lets us:
- write down the design as a semantic gradient,
- detect if it violates a contradiction threshold,
- and record why and where it failed.

This gives us traceability and semantic coherence with minimal theory overhead.

### 2. Core Objects

| Symbol             | Meaning                                                  | Required PV |
|-------------------|----------------------------------------------------------|-------------|
| $\mathcal{F}$      | Semantic field (where all tension resides)               | ⬡[PV1.1]    |
| $\Xi$              | Contradiction tensor (field tension measure)             | ⬡[PV1.2]    |
| $\Delta$           | Design gradient vector supplied by engineer              | ⬡[PV1.1]    |
| $\mathcal{C}$      | Projection functor (collapse when threshold met)         | ⬡[PV1.3]    |
| $\tau_D$           | Narrative trace written on design collapse               | ⬡[PV2.3]    |
| $R$                | Relevance field (local concern gradient)                 | ⬡[PV1.1]    |
| $\phi_{\text{pre}}$| Pre-agentic teleological vector (collapse direction)     | ⬡[PV1.5]    |
| $\mathcal{P}$      | Projected triad: (subject, agent, addressee)             | ⬡[PV4.2]    |

### 2.1 Trace Dependency Tiers

| Tier         | Artefacts Logged                                           | Typical Engineering Use                            |
|--------------|------------------------------------------------------------|----------------------------------------------------|
| τ-minimal    | $\tau_D$ only                                              | “When did this idea collapse?”                     |
| τ+context    | $\tau_D$ + local $\Xi,\kappa$ snapshot                     | Basic cause mapping or diff inspection             |
| full τ-graph | Linked τ nodes + projected $\phi_{\text{pre}}$, $\mathcal{P}$ | Full design lineage, belief intention, trace replay |

## 3. Collapse Rule for Design Projection

A design gradient $\Delta$ triggers collapse when the local contradiction slope exceeds a threshold:

$$
\left\lVert \nabla_{\!\! \Delta} \Xi \right\rVert > \theta_{\text{design}}
$$

⬡[PV2.2]

This means: *if pushing the design forward steepens contradiction beyond the shared threshold*,  
then the design must either be reframed or delayed (e.g. scaffolded).

When collapse fires, we invoke:

$$
\mathcal{C}: (\mathcal{F}, \Delta) \longrightarrow \mathcal{B}
$$

and a design-trace $\tau_D$ is written into the system's audit structure ⬡[PV2.3].

## 4. What This Enables Now

| Need                                 | How It’s Satisfied                           |
| ------------------------------------ | -------------------------------------------- |
| Trace every failed design decision   | Automatic $\tau_D$ written on collapse       |
| Filter low-coherence designs early   | Use $\left\lVert \nabla_\Delta \Xi \right\rVert$ as tension gate |
| Compare design variants              | Compare projected $\Xi$ gradients            |
| Integrate with constraint engine     | $\tau_D$ and PV-tagged gradients are reusable |

In richer trace modes, the projection also records:

- the directional vector $\phi_{\text{pre}}$ at point of collapse (optional),
- the projected triad $\mathcal{P} = (\mathcal{S}, \bar{\mathcal{A}}, \hat{\mathcal{A}})$ representing subject, agent, and addressee.

These enhance belief accountability and situated provenance.

In richer trace modes, the projection also records:

- the directional vector $\phi_{\text{pre}}$ at the point of collapse,
- the projected triad $\mathcal{P} = (\mathcal{S}, \bar{\mathcal{A}}, \hat{\mathcal{A}})$ representing subject, agent, and addressee.

These enrich the audit trail with pre-collapse intention and responsibility traces, useful for epistemic alignment, rollback coordination, or explanatory debugging.


## 5. Formal Dependencies

| PV Tag     | Role in Structure                                               |
|------------|-----------------------------------------------------------------|
| ⬡[PV1.1]   | Supplies $\mathcal{F}$, $R$, and enables directional $\Delta$   |
| ⬡[PV1.2]   | Supplies contradiction tensor $\Xi$                             |
| ⬡[PV1.3]   | Defines projection functor $\mathcal{C}$                         |
| ⬡[PV1.5]   | Enables pre-agentic directional vector $\phi_{\text{pre}}$      |
| ⬡[PV2.2]   | Collapse threshold pattern                                       |
| ⬡[PV2.3]   | Design-trace schema $\tau_D$                                    |
| ⬡[PV4.2]   | Projected triad for belief accountability $\mathcal{P}$         |

Triadic structure $\mathcal{P}$, when logged, supports retroactive epistemic alignment across modules and agents.

## 6. Sensitivity and Perturbation Mapping

| PV Code   | If it changes …                        | Consequence                                       |
|-----------|----------------------------------------|--------------------------------------------------|
| ⬡[PV1.2]  | Redefine $\Xi$ structure               | Design-tension norms shift; must retune $\theta$ |
| ⬡[PV2.2]  | Collapse rule adjusted                 | Earlier or later collapse triggers               |
| ⬡[PV2.3]  | Trace system changed                   | $\tau_D$ may lose audit sufficiency              |
| ⬡[PV1.5]  | Modify $\phi_{\text{pre}}$             | Directional logs misalign with field dynamics    |
| ⬡[PV4.2]  | Triadic collapse structure modified    | Trace loses relational or agentive coherence     |


## 7. Implementation Notes

- $R$ — Concern field: vector field showing where attention is focused in $\mathcal{F}$
- $\phi_{\text{pre}}$ — Drift vector induced by contradiction and entropy
- $\mathcal{P}$ — Projected agent triad: defines who is implicated in belief

* Engineering teams attach a design-gradient $\Delta$ to any candidate design zone.
* The system evaluates:

$$
\left\lVert \nabla_{\!\! \Delta} \Xi \right\rVert
$$

* If this exceeds $\theta_{\text{design}}$, the system fires $\mathcal{C}$, commits the projection, and logs $\tau_D$.

* If not, the gradient is retained as part of an evolving design, or scheduled for resimulation.

> *No π-stacks, no UCSE, no traversal layers required in this pass.*  
> This enables engineering prototypes to participate immediately in semantic tracing,  
> while remaining upgradable as the architecture matures.

### Glossary Snapshot

- $R$ — Concern field: shows where attention or risk is focusing in $\mathcal{F}$
- $\phi_{\text{pre}}$ — Local collapse drift vector; logs direction collapse emerged from
- $\mathcal{P}$ — Projected triad: identifies belief subject, agent, and implied recipient


## 8. Toward a Gradient-Based Design Grammar (Seed)

This minimal theory enables traceable design collapses. But for semantic engineering to become *expressive*, it needs a grammar: a way to describe, test, and compose design events as operations in meaning space.

This grammar must:
- Describe design events as semantic gradients,
- Express tension conditions and closure outcomes,
- Represent trace relationships across projections,
- Allow constraint-satisfaction procedures to operate symbolically on semantic fields.

Because all design behaviour is expressed through field tension, semantic gradients are the natural substrate for engineering expression. Any design language or DSL must ultimately reduce to or be interpretable through these gradients.

### Example gradient classes:

- Modularity pressure — the degree to which a submodule can be collapsed without affecting adjacent $\Xi$ gradients.
- Closure tension — sharpness of $\nabla_{\Delta} \Xi$ within design zones; predicts likely collapse.
- Trace volatility — how fragile the projected trace $\tau_D$ is to nearby perturbations or edits.

Future work should explore how these gradient classes behave under:
- Composition,
- Projection,
- Reprojection,
- and rhetorical modulation.

This is the foundation of a future Design Grammar for Semantic Engineering, where the language of design can be probed, tested, and stabilised through its tensorial expression.

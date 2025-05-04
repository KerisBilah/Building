---
title: Foundational Priors
aliases:
  - Architectural Priors
  - Constraint Assumptions
  - Rhetorical Constraint Model
tags:
  - semantic-architecture
  - foundational
  - constraint-engine
  - rhetorical-priors
  - tensor-geometry
created: 2025-04-21
updated: 2025-04-21
status: stable
project: semantic-agency-architecture
author: Bee
priority: high
related:
  - appendix-a-architectural-assumptions
  - appendix-b-structural-assumptions
  - two-worlds-core
  - constraint-engine-notes
version: 1.2.0
version-notes: v1.2.0 — Introduced formal definition of $\text{TRL}_\text{inf}$ as the Prolog-style inference logic within the Tensor Resolution Layer. Updated Architectural Assumptions and sensitivity table (Appendix A) to reflect its role in semantic traversal, contradiction amplification, and pre-resolution field preparation. Maintains coherence with $\pi_i$-modulated constraint dynamics and preserves functorial structure of $\mathcal{C}$.
---
# Foundational Priors v1.2.0

> This document outlines the architectural assumptions that govern rhetorical resolution strategies in the semantic agency architecture. These priors define the valid space in which contradiction can be resolved, closure can occur, and belief-level commitments can emerge.

## Core Entities

Let:
- $\mathcal{F}$: The fuzzy semantic manifold — a high-dimensional tensor space encoding distributed meaning, salience, and contradiction.
- TRL: Tensor Resolution Layer — a non-destructive logic-based traversal system that prepares $\mathcal{F}$ for projection by surfacing latent contradictions and simplifying incompatible topologies.
- $\mathcal{C}$: Constraint satisfaction engine — resolves contradiction, detects closure, and projects irreducible semantic structures into the belief space $\mathcal{B}$. It is embedded with rhetorical priors $\pi_i$.
- $\mathcal{B}$: Belief space — the space of propositional commitments, agentive structures, and probabilistic inferences.
- $\pi_i$: Rhetorical resolution priors — modular interpretive operators embedded within $\mathcal{C}$ that modulate its resolution behaviour under conditions of contradiction.

## Architectural Assumptions

These assumptions define the behaviour of closure formation, constraint resolution, and recursive feedback from beliefs to meaning.

| Code | Description                                                                                                                                                              |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| (P1) | $\mathcal{C} : \mathcal{F} \to \mathcal{B}$ is a structured functor mapping semantic closures to belief-level commitments.                                               |
| (P2) | Compression failure triggers projection: if $$\kappa + \Xi + \mathcal{E} > \theta$$, closure occurs and $\mathcal{C}$ commits to projection.                             |
| (P3) | Constraint satisfaction is directional: modulated by teleological vector $\phi$ and concern field $R$.                                                                   |
| (P4) | Rhetorical priors $\pi_i$ embedded in $\mathcal{C}$ modulate how closure is achieved, which contradictions are prioritized, and which resolution strategies are favored. |
| (P5) | Semantic closures recursively update the narrative trace $\tau$, influencing future closure thresholds.                                                                  |
| (P6) | Reprojection is permitted: $$\mathcal{C}^{-1} : \mathcal{B} \to \mathcal{F}$$ allows belief-level commitments to deform or pressure the semantic field.                  |
| (P7) | A Tensor Resolution Layer (TRL) prepares $\mathcal{F}$ before projection, surfacing contradictions and simplifying high-dimensional regions into resolve-ready forms.    |

> These assumptions jointly define the interpretive coherence of the architecture. Violation of any assumption may require reclassification of rhetorical priors or a redefinition of closure dynamics.

## Rhetorical Priors and Modulation

Rhetorical priors $\pi_i$ act as interpretive operators internal to $\mathcal{C}$ and modulate its behaviour under contradiction. Each $\pi_i$ may influence:

- Closure preference: Which types of closure (e.g. ontological, affective, pragmatic) are favoured.
- Contradiction interpretation: Whether a contradiction is taken to imply opposition, incompleteness, polysemy, or ambiguity.
- Resolution strategy: Whether to resolve contradiction through synthesis, selection, deferral, or reconfiguration.

Rhetorical priors are not external to computation; they are internal modulating structures, akin to learned priors or control signals within the architecture of $\mathcal{C}$.

### Interaction with the TRL

- The TRL detects high-curvature or topologically inconsistent regions in $\mathcal{F}$.
- These contradictions are flagged but not resolved by the TRL.
- The output of the TRL feeds into $\mathcal{C}$, which then resolves, projects, and modulates the result under the influence of active $\pi_i$.

## Sensitivity Summary

| Assumption | If It Changes...                             | Consequence                                                        |
| ---------- | -------------------------------------------- | ------------------------------------------------------------------ |
| (P1)       | $\mathcal{C}$ loses functorial structure     | Resolution strategies lose internal coherence and transferability  |
| (P2)       | No compression threshold                     | Collapse logic is undefined; $\mathcal{B}$ becomes ungrounded      |
| (P3)       | No teleological or concern-driven modulation | Resolution becomes uniform and inert; no prioritization            |
| (P4)       | $\pi_i$ priors removed                       | Resolution becomes unframed; interpretive strategy is lost         |
| (P5)       | No $\tau$ trace                              | Narrative memory is lost; recursive closure tuning disappears      |
| (P6)       | No reprojection                              | Beliefs do not influence semantics; agency is one-directional      |
| (P7)       | TRL misconfigured or absent                  | Contradictions remain latent; projection becomes unstable or noisy |


## Summary

This document provides the structural assumptions and modulation framework required for rhetorical strategies to operate meaningfully within the semantic agency architecture. At the heart of this system is the interplay between the TRL, which exposes contradiction; the constraint engine $\mathcal{C}$, which resolves it; and the rhetorical priors $\pi_i$, which frame the meaning of that resolution.


## Appendix A: Architectural Assumptions (v1.2.0)

This appendix formally enumerates the structural assumptions upon which this document depends. They define the valid operational space for the constraint satisfaction engine, the rhetorical strategies $\pi_i$, and the full resolution chain from $\mathcal{F}$ to $\mathcal{B}$.

### Core Architectural Entities

- $\mathcal{F}$: The fuzzy semantic manifold — a high-dimensional tensor space encoding distributed meaning, salience, and contradiction.
- TRL: Tensor Resolution Layer — a non-destructive traversal system that prepares $\mathcal{F}$ for projection by surfacing contradictions and simplifying topological structure.
- $\mathcal{C}$: The constraint satisfaction engine — the core system that resolves contradictions, computes closure, and projects results into $\mathcal{B}$. It is embedded with rhetorical priors $\pi_i$.
- $\mathcal{B}$: The belief space — a space of propositional commitments, agentive models, and probabilistic inferences.
- $\pi_i$: Rhetorical resolution priors — modular operators that guide the behaviour of $\mathcal{C}$ under contradiction.

### Formal Dependencies

| Assumption | Description                                                                                                                                                                                                                                                        |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| (P1)   | $\mathcal{C} : \mathcal{F} \to \mathcal{B}$ is a structured functor mapping semantic closures to beliefs.                                                                                                                                                          |
| (P2)   | Compression failure triggers projection: if $$\kappa + \Xi + \mathcal{E} > \theta$$, closure occurs.                                                                                                                                                               |
| (P3)   | Constraint satisfaction is directional: guided by the teleological vector $\phi$ and concern field $R$.                                                                                                                                                            |
| (P4)   | Rhetorical priors $\pi_i$ are embedded in $\mathcal{C}$ and modulate resolution behaviour under contradiction.                                                                                                                                                     |
| (P5)   | Semantic closures update the narrative trace $\tau$ recursively.                                                                                                                                                                                                   |
| (P6)   | A partial inverse $$\mathcal{C}^{-1} : \mathcal{B} \to \mathcal{F}$$ allows reprojection from belief to meaning.                                                                                                                                                   |
| (P7)   | A Tensor Resolution Layer (TRL) operates prior to $\mathcal{C}$ and prepares $\mathcal{F}$ by exposing latent contradictions and simplifying configuration.                                                                                                        |
| (P8)   | $\text{TRL}_\text{inf}$ performs semantic traversal and amplification of $\mathcal{F}$ using contradiction traces $\Xi$, curvature $\kappa$, concern $R$, and narrative history $\tau$. It prepares regions for resolution but does not perform projection itself. |

### Sensitivity Table

| Assumption | If It Changes...                            | Consequence                                                                                                         |
| ---------- | ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| (P1)       | $\mathcal{C}$ loses functorial structure    | Resolution priors lose context and coherence                                                                        |
| (P2)       | No compression threshold                    | Collapse logic undefined; $\mathcal{B}$ underdefined                                                                |
| (P3)       | No teleological flow or concern modulation  | All strategies reduce to ad hoc selection                                                                           |
| (P4)       | $\pi_i$ not implemented                     | Resolution becomes structurally blind to interpretive frames                                                        |
| (P5)       | No $\tau$ trace                             | System loses narrative memory and rhetorical accumulation                                                           |
| (P6)       | No reprojection                             | No feedback from action to meaning; semantic field decouples                                                        |
| (P7)       | $\text{TRL}$ misconfigured or absent        | High-dimensional contradictions remain latent; resolution becomes noisy or unreliable                               |
| (P8)       | $\text{TRL}_\text{inf}$ removed or weakened | System becomes unable to prepare semantic material for projection; resolution becomes brittle, ungrounded, or noisy |

> Changes to any of these assumptions require a re-audit of all $\pi_i$ definitions and the validity of the constraint-resolution strategies described herein. The TRL is especially critical for ensuring that $\mathcal{C}$ operates on a simplified, contradiction-aware subset of $\mathcal{F}$.

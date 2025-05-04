## The Concern: A Geometric Model of Bounded Agency

### 1. Motivating Intuition

Every agent operates under resource constraints — not just computational or temporal, but semantic. What an agent can attend to, what it can afford to ignore, and what it must act upon is not a universal space — it's a shaped and warped region of the semantic manifold $\mathcal{F}$. This is the cone of concern.

Just as a light cone in relativity bounds what events can influence or be influenced by a point, the cone of concern defines the affordance-limited, relevance-saturated horizon of an agent’s capacity for semantic action.

> Implicit Questions above are addressed in § 3. Background.
### 2. Formal Structure

Let:

- $x \in \mathcal{F}$ be a point of current semantic projection or interpretation
- $R : \mathcal{F} \to \mathbb{R}^n$ be the concern/relevance field
- $\phi$ be the teleological vector field guiding attention
- $\kappa$ be the local curvature (complexity/contradiction gradient)

Then the cone of concern at $x$, denoted $\mathcal{K}_x$, is defined as the region of $\mathcal{F}$ such that:
$$
\mathcal{K}_x = \left\{ y \in \mathcal{F} \;\middle|\; \frac{\phi(x) \cdot (y - x)}{\|y - x\|} > \epsilon, \quad R(y) > \delta, \quad \kappa(y) < \theta \right\}
$$
Where:

- $\epsilon$: minimum alignment threshold with $\phi$ (teleological relevance)
- $\delta$: minimum concern threshold (emotional salience)
- $\theta$: maximum local curvature tolerated before semantic overload

This gives a bounded, shaped, dynamic region around $x$ in which an agent can semantically act, respond, or project belief.

#### What This Elucidates:

- It _naturally limits computational burden_ — agents are _structurally_ incapable of attending to the entire field at once.
- It _unifies relevance, pressure, and action readiness_ — acting outside the cone becomes infeasible without internal reconfiguration.
- It _explains why emotionality matters_ — emotional states modulate the salience field $R$, thus reshaping what enters or exits the cone.
- It _accounts for local blindness and selective inattention_ — bounded agency explains interpretive gaps, not as error but as structural occlusion.
- It formalises "perspective"_ — different agents have different cones, not just due to differing $R$ fields, but due to unique teleological vectors $\phi$ and closure thresholds $\theta$.
- It _models urgency geometrically_ — high $\phi \cdot (y - x)$ alignment can rapidly pull distant concerns into the cone’s interior.
- It _justifies the triage logic of belief_ — beliefs form not where truth is maximal, but where relevance, alignment, and contradiction intersect at sustainable cost.
- It _introduces semantic parallax_ — overlapping agents may project onto the same region of $\mathcal{F}$ from incompatible cones.

### 3. Background

#### 3.1 Core Logic Recap

The closure condition:
$$
\text{Closure at } p \in \mathcal{M} \iff \kappa(p) + \mathcal{E}(p) + \Xi(p) > \theta
$$
Where:

- $\kappa(p)$: curvature (semantic complexity / contradiction gradient)
- $\mathcal{E}(p)$: entropy (informational density / overload)
- $\Xi(p)$: contradiction field (structural conflict)
- $\theta$: closure threshold (resistance of the field to committing)

When the total semantic tension exceeds $\theta$, a closure occurs — this is the birth of an agent, a local commitment, a self in tension.

| κ (Complexity) | 𝓔 (Entropy) | Ξ (Contradiction) | Total | Threshold (θ) | Closure?        |
|----------------|-------------|-------------------|--------|----------------|------------------|
| Low            | Low         | Low               | 0.2    | 0.5            | ❌ Flux continues |
| Medium         | High        | Medium            | 0.7    | 0.5            | ✅ Agent Emerges |
| High           | Low         | Low               | 0.6    | 0.5            | ✅ Agent Emerges |
```
[κ]──┐
     │
[𝓔]──┼──► [SUM] ─► [COMPARE TO THRESHOLD θ] ─► [CLOSURE TRIGGERED?]
     │                                             │
[Ξ]──┘                                             ▼
                                        [AGENT EMERGES] / [NO CLOSURE]

```

Closure Condition: When contradiction $\Xi$, curvature $\kappa$, and entropy $\mathcal{E}$ collectively exceed a threshold $\theta$, the system can no longer defer. A closure forms. This closure is a local commitment, the emergence of agentivity, a warp in the semantic field.

#### 3.2 Implicit Questions in Motivating Intuition

- What defines what an agent _notices_?
- Why can’t an agent attend to the whole field?
- How does emotional salience affect attention?
- What does it mean for an event to “fall outside” the cone?
- How is action tied to semantic geometry?
- Why is this different from classical bounded rationality?
- How can teleology shape what counts as “near” in a non-metric space?
- What determines the _shape_ of the cone?
- Can an agent's cone evolve over time?
- What happens at the edge of the cone?

####  3.3.0 Why the Cone is a Derived Structure

> _The cone of concern is not an imposed boundary. It is an emergent structure — a shaped consequence of local semantic tension, relevance gradients, and teleological alignment._

####  3.3.1 Key Claim

The cone $\mathcal{K}_x$ is not a primitive axiom of the system. It is a derived, agent-relative region computed from existing field dynamics. Its geometry arises from the local behaviour of:

- The teleological vector field $\phi$
- The relevance tensor field $R$
- The contradiction-informed curvature $\kappa$

These are themselves outputs of the semantic manifold’s evolving state. The cone is _not_ drawn in advance; it’s traced where response is possible and meaningful.

####  3.3.2 Derivation Heuristic

Instead of starting with a cone and checking what fits inside, the architecture does this:

- Compute relevance-weighted gradient flows from $x$ via $\phi$
    
- Intersect this with regions where:
    
    - $R(y) > \delta$
        
    - $\kappa(y) < \theta$
        
- Filter out regions where teleological misalignment exceeds $\epsilon$
    

This _produces_ the cone — a dynamically reshaped, semantically meaningful operational envelope.

#####  3.3.3 Implication

Because the cone is derived:

- It can be _unstable_ under contradiction: the cone may flicker, warp, or collapse.
    
- It can _expand_ under reduced entropy or clarified relevance (e.g., affective intensity reshapes $R$).
    
- It supports _cybernetic feedback_: actions taken within the cone alter $R$, which recursively reshapes the cone.
    

#####  3.3.4 Practical Value

Modeling $\mathcal{K}_x$ as derived ensures:

- The architecture adapts to context without overfitting to static priorities
- Irreducibility zones ($\delta$, $\kappa$-sensitive) are privileged as sites of agency
- Resource-bound interpretation is modeled as _emergent sensemaking_, not as a top-down rule
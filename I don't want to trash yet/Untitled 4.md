## Phase I: Establish the Expressive Space of Rhetorical Priors

#### Goal: Build a compositional, extensible, and interpretable system of πi\pi_iπi​ priors.

This means:
- Defining the algebra: how do priors combine, override, nest, or conflict?
- Describing signatures: each prior has a _geometric effect_, a _modulation profile_ on contradiction resolution, and a possible _teleological influence_.
- Establishing classes: some priors are existential (what is), some ethical (what matters), some procedural (how to resolve).

We can think of priors in terms of:

text

CopyEdit

`πᵢ : Ξ × R × φ × τ → δ𝓒`

Which means: for a given contradiction, concern gradient, teleology, and narrative trace, each prior outputs a modification to the constraint resolution pathway.

Think of this like establishing a rhetorical modulation layer—a field of knobs and levers for shaping how collapse occurs.

## Phase II: Toward Adaptive Priors and Interpretive DNA

#### Goal: Let rhetorical disposition be modulated by learning, experience, or context.

This is where we start treating the priors themselves as:
- Partially plastic (modifiable over time),
- Context-sensitive (adjusted by agent role, environment, or social signals),
- And possibly learned (through closure history or error signals).

You said:

> It’s not a generative system, it’s listening.

Exactly—and what does an _ear_ do but develop resonance profiles? You could model this as:
- Narrative tuning: past closures warp the rhetorical field—what the agent is now more likely to “hear” or “resolve”
- Closure plasticity: frequent types of contradiction shape which priors get reinforced (à la Hebbian inference)
- Self-modulating constraint logic: the agent becomes rhetorically attuned, not by logic alone but by lived deformation history

Think of this as developing rhetorical DNA—not fixed, but epigenetically responsive to narrative and interactional experience.

## Phase III: Shepard-like Generalization in the Semantic Field

#### Goal: Implement geometric generalization strategies as resolution priors.

This is where your Shepard reference shines:

- Use distance decay laws or topological neighbourhood structures to model how resolution strategies generalise from one configuration to another.
    
- These could manifest as:
    - Weighted influence maps over contradiction zones
    - Curvature-sensitive similarity functions (e.g. high-curvature zones propagate different generalization dynamics than flat ones)
    - Attention-like spread over semantic fields

You now have a language for priors that can:

- Favour closeness (Shepard-style exponential decay),
- Prioritise curvature similarity (resolve contradictions in similar "shaped" zones),
- Or encode symbolic form within geometric context (e.g. category-preserving topologies).

This is the bridge to building interpreters that evolve, differentiate, and specialize without ever leaving the space of geometry and constraint.

## Generalisation Principles and Heuristics

### 1. Shepard's Exponential Law of Generalisation

Formalism:
$$
\text{Pr}(y \mid x) = e^{-d(x, y)}
$$

Context:  
Probability of generalising from $x$ to $y$ decays exponentially with their psychological distance in a similarity space.

Pros:
- Empirically grounded in psychological experiments.
- Smooth, continuous model of generalisation.

Cons:
- Assumes fixed similarity metric.
- Doesn’t account for learning, context, or exemplar variability.

---

### 2. Tenenbaum & Griffiths’ Size Principle

Formalism:
$$
\text{Pr}(E \mid H) \propto \frac{1}{\text{size}(H)^{|n|}}
$$

Context:  
Given $|n|$ examples, hypotheses referring to smaller categories are preferred. Explains the "suspicious coincidence" effect.

Pros:
- Explains undergeneralisation with more examples.
- Formalises rational inductive bias toward specific categories.

Cons:
- Disregards similarity as explanatorily relevant.
- Semantically underdefined notion of "size".



### 3. Carnap’s $\gamma$-Rule

Formalism:
$$
\text{Pr}(H_{C_i}) = \frac{\text{size}(C_i)}{\text{size}(\text{CS})}
$$

Context:  
Used to assign prior probabilities based on region size in conceptual space (CS), assuming equiprobability in absence of evidence.

Pros:
- Semantically grounded prior.
- Avoids arbitrariness of carving-up hypothesis space.

Cons:
- Static; doesn’t model learning or evidence-based updates.
- Ignores pragmatic usage effects.


### 4. Decock et al.'s Geometric Principle of Indifference (gPOI)

Formalism:
$$
\mu^*(C_i) = \frac{\mu(C_i)}{\mu(\text{CS})}
$$

Context:  
Lebesgue-normalised measure used to define prior belief over concept regions in conceptual space.

Pros:
- Geometrically precise.
- Semantically interpretable via conceptual similarity space.

Cons:
- Doesn’t accommodate dynamic learning.
- Misses pragmatic frequency effects.



### 5. Geometric Size Principle *(Extension of T&G via conceptual spaces)*

Formalism (Single exemplar):
$$
\text{Pr}(e_i \mid H_{\langle C_i, L \rangle}) = \frac{\mu(e_i \cap C_i)}{\mu(C_i)}
$$

Formalism (Multiple exemplars):
$$
\text{Pr}(E = \langle e_1, ..., e_n \rangle \mid E \in C_i) \propto \frac{\mu^*(E \cap C_i)}{\mu^*(C_i)}
$$

Context:  
Likelihood derived from spatial overlap in conceptual space; incorporates similarity, exemplar variability, and frequency.

Pros:
- Transparent semantics via geometry.
- Captures dynamic exemplar variability.
- Accounts for both under- and overgeneralisation.

Cons:
- Requires defined conceptual space geometry.
- Still developing integration with pragmatic inference.


### 6. Convexity Constraint (Conceptual Spaces Theory)

Principle:  
If two items belong to the same category, then all points on the line segment between them also do.

Context:  
Used to exclude gerrymandered categories like “tulip in the afternoon”.

Pros:
- Explains preference for natural, projectible categories.
- Helps resolve Goodman’s new riddle of induction.

Cons:
- Requires a meaningful similarity metric.
- Not sufficient on its own to guide inference.


### 7. Voronoi Tessellation (Category acquisition mechanism)

Mechanism:  
Conceptual space is partitioned into convex cells based on distance to category prototypes.

Context:  
Explains generalisation and categorisation by spatial proximity to prototypes.

Pros:
- Explains overgeneralisation via spatial expansion.
- Compatible with continuous learning.

Cons:
- Prototype selection may be arbitrary.
- Less effective for multimodal or non-convex categories.

# Summary of Formalised Conceptual Spaces with a Geometric Representation of Correlations 
Lucas Bechberger and Kai-Uwe Kühnberger

## Motivation

The paper formalises and implements Gärdenfors’ conceptual spaces framework using:
- Fuzzy star-shaped sets (instead of convex sets)
- Geometric encoding of correlations
- Operations on concepts: intersection, union, projection, etc.
- Aimed toward symbol grounding and concept formation from perceptual data

## Core Problem

- Convexity + Manhattan metric leads to axis-aligned cuboids
- This prevents encoding correlations (e.g., age-height in children)
- Solution: Use star-shaped sets with central prototypes

## Mathematical Foundations

### Conceptual Space

- Quality dimensions: $d \in D$
- Domains: $\delta \subseteq D$

Intra-domain distance (Euclidean):

$$
d^\delta_E(x, y, W_\delta) = \sqrt{ \sum_{d \in \delta} w_d \cdot |x_d - y_d|^2 }
$$

Overall space (Manhattan sum of intra-domain distances):

$$
d_C(x, y, W) = \sum_{\delta \in \Delta} w_\delta \cdot d^\delta_E(x, y, W_\delta)
$$

Similarity:

$$
\text{Sim}(x, y) = e^{-c \cdot d(x, y)}
$$



### Star-Shaped Sets

A set $S \subseteq CS$ is star-shaped under $d$ with respect to $P \subseteq S$ if:

$$
\forall p \in P, z \in S, y \in CS: \quad B_d(p, y, z) \Rightarrow y \in S
$$



## Fuzzy Simple Star-Shaped Sets

### Cuboid

Defined on a subset of dimensions:

$$
C = \{ x \in CS \mid \forall d \in D : p_d^- \leq x_d \leq p_d^+ \}
$$

### Core

Union of overlapping cuboids with nonempty intersection:

$$
S = \bigcup_{i=1}^m C_i, \quad P = \bigcap_{i=1}^m C_i \neq \emptyset
$$

### Fuzzy Concept

Defined as:

$$
\tilde{S} = \langle S, \mu_0, c, W \rangle
$$

Membership function:

$$
\mu_{\tilde{S}}(x) = \mu_0 \cdot \max_{y \in S} e^{-c \cdot d_C(x, y, W)}
$$

Alpha-cut:

$$
S^\alpha = \{ x \in CS \mid \mu_{\tilde{S}}(x) \geq \alpha \}
$$


## Concept Operations

### Intersection

If $P_1 \cap P_2 = \emptyset$, repair by extending cuboids to meet at $p^*$.

$$
\tilde{S}' = \langle I(S_1, S_2), \mu_0', c', W' \rangle
$$

Where:
- $\mu_0' = \max\{ \alpha \mid S_1^\alpha \cap S_2^\alpha \neq \emptyset \}$


### Unification

Union of cuboids, with repair if needed:

$$
\tilde{S}' = \langle S_1 \cup S_2, \max(\mu_0^{(1)}, \mu_0^{(2)}), \min(c^{(1)}, c^{(2)}), W' \rangle
$$


### Projection

Project concept $\tilde{S}$ onto domain subset $S' \subseteq S$


### Axis-Aligned Cut

Split concept along dimension $d$ at value $v$


## Concept Size

Defined via fuzzy set measure:

$$
M(\tilde{S}) = \int_0^1 \text{Vol}(S^\alpha) \, d\alpha
$$

Volume of $\alpha$-cut:

$$
V(C^\alpha) = \sum_{i=0}^n \sum_{\{d_1, ..., d_i\} \subset D} \left( \prod_{d \notin \{d_1,...,d_i\}} b_d \right) \cdot V_{\text{ball}}(r, \{d_1,...,d_i\}, W)
$$

with $r = -\frac{1}{c} \ln \frac{\alpha}{\mu_0}$


## Subsethood and Implication

Subsethood:

$$
\text{Sub}(\tilde{S}_1, \tilde{S}_2) = \frac{M(\tilde{S}_1 \cap \tilde{S}_2)}{M(\tilde{S}_1)}
$$

Implication:

$$
\text{Impl}(\tilde{S}_1, \tilde{S}_2) = \text{Sub}(\tilde{S}_1, \tilde{S}_2)
$$


## Similarity and Betweenness

- Similarity between concepts based on prototype distance and weights
- Betweenness is binary, based on midpoints

## Implementation

- Python 2.7 code available on GitHub
- Toy example: fruit space with $\delta_\text{color}$, $\delta_\text{shape}$, $\delta_\text{taste}$

## Future Work

- Refine similarity/betweenness
- Develop concept formation (incremental clustering, hierarchy)
- Integrate deep learning for domain construction
- Apply in symbol grounding architecture

## Conclusion

This formalisation:
- Provides fuzzy geometric representation of concepts
- Handles cross-domain correlations
- Supports a rich algebra of operations
- Is computationally tractable and implementable



## Section 2.1 – Introduction
### Core Summary
The chapter introduces a debate about how humans generalise from stimuli.
Shepard (1987) proposed the Universal Law of generalisation (ULG) based on psychological similarity—generalisation is more likely the more similar two stimuli are.
Tenenbaum & Griffiths (2001) (T&G) extended this with a Bayesian model, arguing:
- generalisation can be computed from multiple examples (not just pairwise).    - Their model unifies Shepard’s distance-based similarity with Tversky’s feature-based model, but...
 - They downplay the need for similarity itself, treating probabilities as primary.
The chapter’s main thesis: Conceptual Spaces Theory (Gärdenfors et al.) can mediate between Shepard and T&G, maintaining the cognitive plausibility of similarity while preserving the Bayesian formalism.
###  Key Conceptual Tension
- Shepard: similarity → generalisation
- T&G: probabilities → generalisation (similarity optional or derived)
- Author’s proposal: conceptual spaces can embed similarity within Bayesian inference, preserving Shepard’s psychological realism while enhancing T&G’s formal power.
###  Terminological/Formal Highlights
- Similarity Space: multi-dimensional psychological space where stimulus similarity is represented as spatial proximity.
- Size Principle (to come in 2.3): core idea in T&G’s model, where smaller categories are more likely to generate observed examples.
- Conceptual Spaces: geometric models of concepts (not yet formalised here), used to represent similarity in a structured, cognitively plausible way.
###  Limitations/Critique
- The Bayesian model’s abstraction dismisses psychological similarity as non-essential, which the author argues:
    - Reduces semantic interpretability.
    - Misses important cognitive constraints.
- Shepard’s model, meanwhile, is limited to single-exemplar generalisation and assumes convex, symmetrical, and equal-probability category spaces—idealised and perhaps cognitively unrealistic.
## Section 2.2 – Shepard’s Universal Law of generalisation

###  Core Summary
- Shepard’s goal: Like Newton’s law of gravity, define a universal law for how organisms generalise behaviors across stimuli.
- Proposed the Universal Law of generalisation (ULG):
    > The probability of generalising from stimulus _i_ to _j_ is an exponentially decreasing function of the psychological distance between them.
###  Mathematical Formalism
- Let $g_{ij}$ be the probability of generalising from $i$ to $j$.
- Let $d_{ij}$ be the psychological distance between stimuli.
- Then:
$$
  g_{ij} \propto e^{-k \cdot d_{ij}}
  $$
  where $k$ is a scaling constant.
- Distance $d_{ij}$ is measured in a multi-dimensional similarity space (typically using City-block (L1) or Euclidean (L2) distance).
###  Two Major Insights
1. Uniformity: generalisation gradients are invariant across species and stimuli—what matters is perceived psychological distance, not physical metrics.
2. Measurability: Psychological similarity space is governed by a Minkowski metric—distances like L1 or L2 apply.
###  Conceptual Contributions
- generalisation is cognitive, not just a failure of discrimination (as in behaviorism).
- Similarity can be subjective: it depends on how we _perceive_ rather than how things _physically are_.
- Introduces the idea of first-order similarity (between world and mind) vs. second-order similarity (within mental representations).
### Formal Assumptions in Shepard's Model
- Category regions in similarity space are:
    - (i) Equally probable in location.
    - (ii) Size-distributed via a known density (enabling probabilistic modeling).
    - (iii) Convex, bounded, symmetric (imposing formal constraints on category shape).
###  Limitations/Critique
- Only single-exemplar generalisation.
- Doesn’t account for category internal structure, e.g., prototype effects (Rosch).
- Assumes idealised geometry—real-world categories may be messier.
- Psychological distance must be inferred, not directly observed; subjective similarity judgments may vary.
##  Connecting Thread: Why It Matters
This debate isn't just technical—it's about what kind of mental architecture we assume for categorization:
- Is similarity an irreducible cognitive mechanism?
- Or can all **generalisation** be derived from abstract probabilistic reasoning?
The author sides with Shepard (and later Gärdenfors), arguing that similarity is fundamental, and proposes that conceptual spaces can offer a way to reconcile formal probabilistic models with cognitive plausibility.
## **Section 2.3 – Tenenbaum and Griffiths’ Size Principle**
### **Core Summary**
Tenenbaum and Griffiths (T&G) extend Shepard’s Universal Law of Generalization by:
1. Introducing **Bayesian inference** into generalization modeling.
2. Proposing the **Size Principle** as a formal account of how **category size** and **number of examples** affect generalization.
3. Arguing that **psychological similarity** is **not necessary** for modeling generalization—probability is enough.
### **1. Bayesian Generalization Framework**

T&G frame categorization as **Bayesian inference**, where a learner updates their belief about a hypothesis HHH given evidence EEE:
$$
\Pr(H|E) = \frac{\Pr(E|H) \cdot \Pr(H)}{\Pr(E)}
$$
- $Pr⁡(H∣E)\Pr(H|E)Pr(H∣E):$ Posterior probability of hypothesis $H$ given evidence $E$
- $Pr⁡(H)\Pr(H)Pr(H):$ Prior probability of $H$
- $Pr⁡(E∣H)\Pr(E|H)Pr(E∣H):$ Likelihood of observing $E$ given $H$
- $Pr⁡(E)\Pr(E)Pr(E):$ Evidence (normalizing constant)

In their model, the **key innovation** is how they **redefine the likelihood** term using the **Size Principle**.
### **2. The Size Principle: Formalism & Intuition**
#### **Formal Statement**:
If a learner observes $n$ examples consistent with a hypothesis $H_C$​, then:
$$
\Pr(E | H_C) \propto \frac{1}{\text{size}(H_C)^{|n|}} \tag{2.1}
$$
- $\text{size}(H_C)$: Number (or measure) of items in the category $H_C$
- $|n|$: Number of observed examples
#### **Interpretation**:
- The more examples you have, the **more suspicious** it becomes that they all fall in a large category _by chance_.
- Smaller categories are **preferred** because they make the data **more likely** under the assumption of **random sampling**.
- This is what Xu and Tenenbaum (2007) call the **“suspicious coincidence” effect**.
#### **Example** (from Xu & Tenenbaum):
Three examples of Dalmatians are labeled as “fep.” Consider three hypotheses:
- $H_1$: ‘fep’ = Dalmatians
- $H_2$​: ‘fep’ = Dogs
- $H_3$​: ‘fep’ = White-with-black-dots things
Then, since:
$$ \text{size}(H_1) < \text{size}(H_2) < \text{size}(H_3) $$
we get:
$$
\Pr(E|H_1) > \Pr(E|H_2) > \Pr(E|H_3)
$$
###  **3. Formal Independence from Similarity**
T&G argue that since:
- Probabilities can be calculated using either **distance metrics** (Shepard) or **set-theoretic features** (Tversky),
- And both approaches yield **equivalent likelihoods**,
...then **generalization does not require any particular notion of similarity**.
They write:
> _“Interesting consequences nonetheless follow just from the hypothesis that similarity somehow depends on generalization...”_ (T&G 2001)

This leads them to **reverse Shepard’s logic**:
- Shepard: **similarity → generalization**
- T&G: **generalization → similarity (maybe)**
## **2.3.1 Advantages Over Shepard’s Model**
T&G’s model **improves on Shepard** in two major ways:
### 1. **Accounts for Multiple Examples**
- **Shepard**: only generalization from a single exemplar.
- **T&G**: can update beliefs based on multiple instances $x1​,…,x_n​$.
$$
X = \{x_1, \dots, x_n\}
$$
- More examples → **narrower generalization**, due to:
$$
\frac{1}{\text{size}(H_C)^{|n|}}
$$
### 2. **Predicts Sharpened Boundaries**
- As $|n|$ increases, category boundaries **sharpen**.
- Even similar items may **not** be generalized to if they fall **outside** the more precise posterior.
So the model **explains under-generalization**, where a learner becomes more cautious as more data accumulates—something **Shepard’s model can’t explain**.
## **2.4 Problems with T&G’s Model**
### **2.4.1. **Too Quick to Dismiss Similarity**
- The **independence from specific similarity models** doesn’t justify dismissing **psychological similarity altogether**.
- **Similarity** may still:
    - Explain how **examples cluster**
    - Mediate **perceptual representations**
    - Be necessary to define **exemplar variability**
Without similarity, it’s unclear **what the learner's belief is _about_**—a conceptual gap.
### 2.4.2. **Semantic Opacity**
- Eq. (2.1) lacks reference to **evidence $E$** on the $RHS$.
- Raises the question: what does the learner's belief actually represent?
- Shepard offers a **distance-based internal structure**; T&G don’t offer an alternative.

### 2.4.3. **Undergeneralization Risk**
- The size principle favors **smaller categories**:
$$
\Pr(E | H) \propto \frac{1}{\text{size}(H)^{|n|}}
$$
- So the learner might generalize too narrowly—e.g., thinking “dax” only means **yellow tulips**, not all tulips.
- But in practice, learners (especially children) often **overgeneralize**.

**T&G’s model can’t explain this without additional mechanisms**—a problem for its empirical adequacy.
**Summary of Section 2.3 and 2.4**

| Aspect                      | Shepard (ULG)                        | Tenenbaum & Griffiths (Bayesian + Size Principle)       |
|----------------------------|--------------------------------------|--------------------------------------------------------|
| **Core Principle**         | Similarity drives generalization     | Probabilities drive generalization                     |
| **Mathematical Tool**      | Exponential decay over distance      | Bayesian inference with size-based likelihood          |
| **Handles Multiple Examples?** | ❌ No                              | ✅ Yes                                                  |
| **Grounded in Similarity?**    | ✅ Yes                            | ❌ Not required                                         |
| **Explains Undergeneralization?** | ❌ No                          | ✅ Yes (via size principle)                             |
| **Explains Overgeneralization?** | ✅ Sometimes                   | ❌ Not well                                             |
| **Key Critique**           | Lacks multiple-example reasoning     | Semantically opaque; dismisses similarity too fast     |
## **Section 2.5 – A Geometric Principle of Categorisation**

### **Core Thesis**
By embedding **Bayesian inference** within the framework of **conceptual spaces**, we can:
- **Resolve ambiguities** in T&G’s size principle.
- **Preserve similarity** as a cognitive foundation (contra T&G).
- **Solve the “different carvings-up” problem** in probabilistic reasoning.
- Enrich categorisation models with **semantic and geometric precision**, e.g., via convexity.
## **2.5.1 Decock et al.’s Geometric Principle of Indifference (gPOI)**

### Problem: Different Carvings-Up

The **standard Principle of Indifference (sPOI)** says:
> When no evidence favors one hypothesis over another, assign **equal probabilities** to all.

But this leads to **incoherence** when hypothesis spaces are **carved up differently**. For example:
- Hypothesis space A:
$$
H = \{ H_1 = \text{red},\ H_2 = \text{any other color} \}
$$
Hypothesis space B:
$$
H = \{ H_1 = \text{red},\ H_3 = \text{blue},\ H_2 = \text{any other color} \}
$$

Same event $H_1$​, but different **assigned priors** depending on the carve-up. This is **irrational**.
### Solution: Conceptual Spaces as Geometric Basis

Conceptual spaces provide a **structured hypothesis space** grounded in similarity:
- A **conceptual space** consists of **quality dimensions** (e.g. hue, size, shape).
- Objects are represented as **vectors** in this space.
- **Distance = dissimilarity**, and **regions = categories**.

### Formalism: Carnap’s γ-rule
To assign priors based on **region size** in a conceptual space:
$$
\Pr(H_{C_i}) = \frac{\text{size}(\text{region}_{C_i})}{\text{size}(CS)} \tag{2.2}
$$
This avoids the carving-up problem because the **region size is fixed** by the geometry.
### Refinement: Decock et al.’s Lebesgue Measure
Use the **Lebesgue measure** μ\muμ to calculate the size of regions more precisely:
$$
\mu^*(C_i) = \frac{\mu(C_i)}{\mu(CS)} \tag{2.3}
$$
Where:
- $\mu^*(C_i)$: Normalized measure = prior probability
- $\mu(C_i)$: Area/volume of category region $C_i$
- $\mu: Area/volume of the total conceptual space
This allows **objective priors** and semantically grounded probability assignments.
## **2.5.2 Going Beyond the Size Principle**
### Step 1: Link to Size Principle
The original size principle (T&G):
$$
\Pr(E | H_C) \propto \frac{1}{\text{size}(H_C)^{|n|}} \tag{2.1}
$$
Compared to Carnap’s γ-rule:
$$
\Pr(H_C) = \frac{\text{size}(H_C)}{\text{size}(CS)} \tag{2.2}
$$

**Difference**:
- Eq. 2.1 uses **inverse size** in likelihood
- Eq. 2.2 uses **direct size** in priors
We now use the **geometry of concepts** to reinterpret Eq. 2.1 more precisely, resolving semantic opacity.
### New Proposal: Geometric Likelihood Function
A refined geometric version of the likelihood:
$$
\Pr(e_i | H_{\langle C_i, L \rangle}) = \frac{\mu(e_i \cap C_i)}{\mu(C_i)} \tag{2.4}
$$
Where:
- $e_i$: Observed exemplar
- $C_i$​: Candidate category region
- $\mu(e_i \cap C_i)$: Overlap between evidence and category
- $\mu(C_i)$μ(Ci​)$: Size of category region
This captures the **match between evidence and concept** as a **proportion of spatial overlap**.
### Advantages Over Eq. 2.1
1. **Recovers similarity**: Evidence $e_i$​ is interpreted in terms of distance in conceptual space.
2. **Clarifies semantics**: $C_i$ has geometric structure, not abstract label space.
3. **Evidence is explicit**: Eq. 2.4 makes the role of $e_i$​ visible—missing from Eq. 2.1.

### Example: Zoey Learns “Azure”
- Evidence:
$$
E = \{ e_1 = \langle \text{blue}_1, \text{‘azure’} \rangle,\ e_2,\ e_3 \}
$$
- Hypotheses:
$$
H_1 = \langle \text{turquoise}, \text{‘azure’} \rangle \\
H_2 = \langle \text{light blue}, \text{‘azure’} \rangle \\
H_3 = \langle \text{blue}, \text{‘azure’} \rangle
$$
Using Eq. 2.4, we evaluate each $H_i$ by the **spatial overlap** of its conceptual region with the observed exemplars.
The hypothesis with **maximum overlap** wins:
$$
\Pr(E | H_3) > \Pr(E | H_2) > \Pr(E | H_1)
$$
## Convexity as a Prior Constraint (Criterion P)
A **key insight** from conceptual spaces theory:
> **Natural categories** are **convex** regions in conceptual space (Criterion P).
- If $x_1,x_2\in C,$ then all points **on the line between them** should also be in CCC.
This helps distinguish between **natural** and **gerrymandered** categories, addressing:
- **Goodman’s “grue” problem**
- **Over-/undergeneralization** in categorization
### Tulip Example: Why Convexity Matters
Evidence:
$$
E = \{ e_1 = \langle \text{white tulip}, \text{‘dax’} \rangle,\ \dots \}
$$
Hypotheses:
$$
H_1 = \text{tulip } \\
H_2 = \text{flower } \\
H_3 = \text{tulip in the afternoon}
$$
- Eq. 2.4 can't distinguish between $H_1$ and $H_3$ (both fit E).
- But $H_3$ is non-convex (it mixes category with time).
- So **prior beliefs** should favor $H_1$​ over $H_3$.
Formally:
$$
\Pr(H_1) > \Pr(H_3)
$$
Because **convex categories** (like tulip) are **projectible**, and thus **easier to infer**.
## Voronoi Tessellation and Overgeneralization

A **convexity-based strategy** for overgeneralization:
- Use **Voronoi tessellation** to divide space around prototypes.
- Each cell = convex region = category.
- New items are assigned to closest prototype.
This explains why learners **sometimes overgeneralize**—they apply labels to all nearby items in convex regions.

🧵 **Recap: Why This Matters**

| Problem                   | T&G’s Size Principle                    | Geometric Extension (Eq. 2.4)                          |
|---------------------------|-----------------------------------------|--------------------------------------------------------|
| **Semantic opacity**      | ✅ Present                              | ❌ Solved via spatial overlap                          |
| **No similarity basis**   | ✅ Present                              | ❌ Solved via distances in conceptual space            |
| **Carvings-up problem**   | ✅ Unresolved                           | ❌ Solved via gPOI (Eqs. 2.2–2.3)                      |
| **Prior constraints**     | ❌ Missing                              | ✅ Convexity (Criterion P)                             |
| **Over/under-generalization** | ❌ Not handled                    | ✅ Addressed via convexity & tessellation              |


## **2.5.3 A Worry for the Geometric Principle of Indifference**
### **The Problem: No Pragmatic Sensitivity**
The **Geometric Principle of Indifference (gPOI)** assumes that:
$$
\mu^*(C_a) = \mu^*(C_b) \Rightarrow \Pr(o \in C_a) = \Pr(o \in C_b)
$$
…if regions $C_a$​ and $C_b$​ have the **same size** in conceptual space.
But this neglects **pragmatic usage frequency**. If:
- $C_a$​ is **commonly used** in language,
- $C_b$ is **rarely used**,
…we intuitively assign higher belief to CaC_aCa​—which **gPOI fails to capture**, since it relies on static region sizes alone.
###  **General Limitation: gPOI is Static**
- Decock et al.'s model represents a **snapshot** of rationality.
- But **learning is dynamic**: beliefs evolve with new evidence.
- We need a model that accommodates **evidence-dependent belief updating**.
### **Proposed Fix: Use the Likelihood (Not Just the Prior)**
Rather than encoding usage frequency in the **prior** (as gPOI tries), encode it in the **likelihood**:
$$
\Pr(H|E) = \frac{\Pr(E|H) \cdot \Pr(H)}{\Pr(E)}
$$
This makes usage history part of the observed evidence.
### **Extended Likelihood Function for Multiple Examples**
To include exemplar frequency and variability:
$$
\Pr(E = \langle e_1, \dots, e_n \rangle \mid E \in C_i) \propto \frac{\mu^*(\langle e_1, \dots, e_n \rangle \cap C_i)}{\mu^*(C_i)} \tag{2.5}
$$
This updates Eq. 2.4 to handle **sequence-based learning** and adjusts beliefs based on **average overlap** between multiple examples and the candidate category.
### **Example: Usage Frequency Matters**
Suppose:
- $E = \langle e_1, \dots, e_{10} \rangle$
- 7 items labeled “dax” fall in $C_a$
- 3 items labeled “fep” fall in $C_b$
Then:
$$
\Pr(E, \text{‘dax’} \mid E \in C_a) = \frac{7}{10} > \Pr(E, \text{‘fep’} \mid E \in C_b) = \frac{3}{10}
$$
Even if $\mu(C_a) = \mu(C_b)$, frequency makes $C_a$​ a **more rational category hypothesis**.
### **Density-Based Interpretation**
- Build a **probability density function** over conceptual space.
- Regions with more **frequent labelings** accumulate higher density.
- Over time, **evidence sharpens** the prediction—favoring categories like CaC_aCa​ not just for size, but for **evidence-based likelihood**.
##  **2.6 Conclusion**

### **Summary of the Debate**

| View                 | Shepard (1987)<br>       | Tenenbaum & Griffiths (2001) |
| -------------------- | ------------------------ | ---------------------------- |
| Role of Similarity   | Primary                  | Derived / Optional           |
| Generalization Basis | Psychological similarity | Bayesian inference           |
### **Synthesis via Conceptual Spaces**
The **theory of conceptual spaces** acts as a **semantic bridge** between these positions by:
- Grounding probabilistic inference in **spatial similarity**,
- Supporting both **similarity-based** and **probabilistic** models of categorization.

### **Three Key Contributions of the Geometric Size Principle**

1. **Semantic Interpretability**:  
    Provides a geometrically meaningful interpretation of Bayesian components:
    - Prior: via Carnap’s γ-rule (Eq. 2.2 / 2.3)
    - Likelihood: via spatial overlap (Eq. 2.4 / 2.5)
2. **Compatibility with Shepard & T&G**:
    - Like T&G: Handles exemplar variability and undergeneralization.
    - Like Shepard: Retains similarity as an explanatory construct.
3. **Additional Constraints from Geometry**:
    - **Convexity** (Criterion P) helps:
        - Favor natural categories over gerrymandered ones.
        - Explain overgeneralization (via Voronoi tessellation).
### **Future Directions**
- **Integrate with objective principles of rationality**.
- **Model conditionalisation dynamically**:
$$
\text{If } \Pr(H|E)_{\text{prior}} = \Pr(H) \Rightarrow \Pr(H)_{\text{updated}} = \Pr_E(H)
$$
- Explore pragmatic inference mechanisms inside geometric–probabilistic models.

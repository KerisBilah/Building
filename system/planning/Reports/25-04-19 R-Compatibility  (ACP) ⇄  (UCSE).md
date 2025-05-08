# Compatibility Report  
Agency as Causal Primitive (ACP) ⇄ Unified Constraint Satisfaction Engine (UCSE)  
*Prepared April 2025*

## 1 Overview  

ACP delivers a *geometric semantics* in which a smooth event‑manifold \(M\) is warped by a concern‑tensor \(\mathcal C\) under agent pressure.  
UCSE supplies an *algorithmic solver* that keeps the high‑order semantic tensor \(T\) in a low‑tension configuration via Partial Tucker Decompositions (PTDs) and mesh‑based heuristics.  

Result: UCSE can be viewed as the micro‑dynamics module that the ACP agent calls each step of its dialectical loop (contradiction → action → synthesis).

## 2 Conceptual Correspondences  

| UCSE construct | ACP counterpart | Comment |
|---|---|---|
| Semantic tensor \(T\) | Local coordinate view of \(\mathcal C\) | Each tensor mode ≅ axis in the concern tensor’s basis. |
| Tensor modes \(M_1\dots M_5\) | Weighted dimensions in \(T_xM\) | Provide explicit sliders for affect, stance, etc. |
| PTD morphism \(\mathrm{PTD}_S:T\!\to\!G\) | Local *warp step* lowering stress in sub‑space \(S\) | PTD ≅ micro‑reconfiguration of \(\mathcal C\). |
| Constraint cycle | ACP dialectic | “Mark Contradiction” ⇔ ACP’s CTM \(>\theta\). |
| Voronoi/Delaunay scaffold | Discrete chart of \(M\) | Mesh adapter bridges smooth math ↔ code. |
| Rolling closure | Moving Markov blanket | Shell drifts if \(\lVert\nabla\Phi\rVert\) stays high. |

## 3 Design Tensions & Options  

| # | Question | Option A (lean) | Option B (rich) |
|---|---|---|---|
| 1 | Scope of PTD: does \(G\) bend \(M\)? | *Local cache* — PTD only summarises; \(\mathcal C\) remains source of geometry. | *Geometry‑affecting* — each PTD updates \(\mathcal C\). |
| 2 | Topology change: may Voronoi cells split/merge? | No — treat metaphor as high curvature. | Yes — cell surgery when residual \(&\) ridge weight spike. |
| 3 | Stress metric: one gauge or many? | Composite scalar  \[ \(\mathrm{Stress} = w_1\|\kappa\| + w_2\mathrm{PTD\_res} + w_3\tau\) \] | Vector of three independent signals. |

### Preferred path (authors’ lean)  
* A1 (local PTD cache)  
* B2 (rare topology change)  
* A3 (single scalar stress)  

This keeps ACP maths simple while letting UCSE flag exceptional events that warrant manifold surgery.

## 4 Implementation Alignment  

1. Mesh adapter    
   Differential operators on \(M\) ↔ discrete exterior calculus over Voronoi/Delaunay mesh.  
2. Stress scalar \(S(x)\)    
   ```math
   S(x)=\alpha\,\|\kappa(x)\| \;+\; \beta\,\mathrm{PTD\_res}(x) \;+\; \gamma\,\tau(x)

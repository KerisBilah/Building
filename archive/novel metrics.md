
# Novel Metrics


### **⬡Metric 9.7: Projection Residual $\rho(\mathcal{A})$**

- **Definition**: The irreducible difference between an agent’s projected image $\hat{\mathcal{A}}$ and the traceable effects of its semantic deformation in $\mathcal{F}$.
    
- **Formula**:
    
    ρ(A)=∥C−1(A^)−A∥δ\rho(\mathcal{A}) = \| \mathcal{C}^{-1}(\hat{\mathcal{A}}) - \mathcal{A} \|_{\delta}ρ(A)=∥C−1(A^)−A∥δ​
    
    where $\mathcal{C}^{-1}$ is a reconstructed estimate and $\delta$ is a distinction metric.
    
- **Use**: Quantifies how much of the agent is _not captured_ in belief-space; a high $\rho$ implies deeper irreducibility and potential for novel action.
    



### **⬡Metric 9.8: Communicative Tension $\theta_{\text{comm}}$**

- **Definition**: Measures the local gradient in the relevance field $R$ induced by the agent-level modulation kernel $\mathcal{M}_{\text{agent}}$.
    
- **Formula**:
    
    θcomm=∥∇(Magent(R)−R)∥\theta_{\text{comm}} = \| \nabla ( \mathcal{M}_{\text{agent}}(R) - R ) \|θcomm​=∥∇(Magent​(R)−R)∥
- **Use**: Indicates rhetorical or affective intensity — how strongly an agent is trying to shape another’s attention. Useful in modeling offers, pleas, resistance.
    



### **⬡Metric 9.9: Agentic Convergence $\chi(\mathcal{A}_i, \mathcal{A}_j)$**

- **Definition**: A probabilistic or field-topological measure of whether two projected agents are being treated as compressible to a single agent-model.
    
- **Formula**:
    
    χ(Ai,Aj)=∥A^i∩A^j∥∥A^i∪A^j∥\chi(\mathcal{A}_i, \mathcal{A}_j) = \frac{ \| \hat{\mathcal{A}}_i \cap \hat{\mathcal{A}}_j \| }{ \| \hat{\mathcal{A}}_i \cup \hat{\mathcal{A}}_j \| }χ(Ai​,Aj​)=∥A^i​∪A^j​∥∥A^i​∩A^j​∥​
- **Use**: Tracks when cooperation or fusion is _interpreted_ by a third agent. High $\chi$ implies potential for compression or modeling fusion.
    



### **⬡Metric 9.10: Modulation Opacity $\omega(\mathcal{A})$**

- **Definition**: How much irreducibility an agent retains after applying its modulation kernel — i.e., how much it reveals vs. conceals in $R'$.
    
- **Formula**:
    
    ω(A)=ρ(A)−ρ′(A)\omega(\mathcal{A}) = \rho(\mathcal{A}) - \rho'(\mathcal{A})ω(A)=ρ(A)−ρ′(A)
    
    where $\rho'$ is the projection residual after modulation.
    
- **Use**: Measures how much “identity” is maintained during communication. High $\omega$ means the agent has expressed while protecting its core.
    

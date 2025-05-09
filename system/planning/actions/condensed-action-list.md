# UCSE / Theory-Stack Master Action Board — generated 2025-05-05

active:
  - id: 001.8
    action: Ensure dual-space UCSE reusability across 𝔽 and 𝔅
    notes: All modules must operate natively in both projections.
  - id: 005.6
    action: Only bump YAML version fields if definitions change
    notes: Pure prose edits don’t justify version increment.

in_progress:
  - id: 001
    action: Integrate Constraint Engine suggestions into UCSE architecture
    added: 2025-04-29
    subtasks_total: 9
    status: in_progress
  - id: 004
    action: Develop “Pre-Agentic Projection and Functorial Collapse” paper
    added: 2025-04-27
    subtasks_total: 6
    status: in_progress
  - id: 005
    action: Align draft theory documents to updated PV schema
    added: 2025-04-27
    subtasks_total: 7
    status: in_progress
  - id: 006
    action: Final prep for Foundational Priors v2.0 & Appendix A v2.0
    added: 2025-04-27
    subtasks_total: 11
    status: in_progress
  - id: 007
    action: Integrate UCSE redraft into Minimal Theory of Agency
    added: 2025-04-27
    subtasks_total: 7
    status: in_progress
  - id: 008
    action: Disambiguate “agent” across all theory documents
    added: 2025-04-27
    subtasks_total: 5
    status: in_progress
  - id: 009
    action: Formalise categorical structure of the semantic architecture
    added: 2025-04-16
    subtasks_total: 6
    status: in_progress

pending:
  # —-- highest-priority work packages —--
  - id: 002
    action: Pre-Agentic Rhetorical & Emotional Modulation (highest)
    added: 2025-04-27
    subtasks_total: 5
    status: planned   # ready to start
  - id: 003
    action: Geometric / topological constraint tools for UCSE (highest)
    added: 2025-04-27
    subtasks_total: 4
    status: planned
  # —-- granular tasks waiting for a kick-off —--
  - id: 001.1
    action: Sketch UCSE Core Architecture (blueprint-level)
  - id: 001.2
    action: Formalise Fallacy Selector Module
  - id: 001.3
    action: Update Foundational Priors & Appendix A with 𝔅 definition
  - id: 004.1
    action: Draft Section 1 — Introduction (paper 004)
  - id: 004.2
    action: Write Section 2 — Pre-Agentic Structures
  - id: 004.3
    action: Formalise Section 3 — Functorial Collapse $F:\! \mathcal{F} \to \mathcal{B}$
  - id: 006.1
    action: Copy Appendix A YAML block into /spec/appendix-a_v2.yaml
  - id: 006.3
    action: Move Cone of Concern diagram into /visual/
  - id: 006.10
    action: Define ⬡[PV1.4] formally (“Reprojection …”)
  - id: 007.6
    action: Propose operator $\mathcal{A}ct^{\dagger}$ for closure events
  - id: 008.2
    action: Harmonisation pass through MTOA
  - id: 008.3
    action: Harmonisation pass through UCSE (April redraft)

planned:
  # (only first few shown; 30 + remain — see original list)
  - id: 001.4
    action: Design Prolog-like backtracking flow engine
  - id: 003.1
    action: Curate geometric/topological operators for UCSE
  - id: 006.2
    action: Add Obsidian Dataview snippet for PV tags
- id: 007.1
  action: Annotate original MTOA draft with insertion points for:
    - Triadic grammar ($\mathcal{P}$)
    - Residual irreducibility ($\eta$)
    - Action conditions and thresholds
  status: complete
  notes: Integration confirmed in *Agency as Causal Primitive v2.0* (Sections 1.3.5, 1.3.7, and 1.5.3).
  - id: 008.1
    action: Draft shared glossary “Typology of Agency”
  - id: 009.1
    action: Define category $\mathcal{F}$ (objects + morphisms)
   … (collapse for brevity)

blocked:
  - id: 006.4
    action: Confirm Foundational Priors v2.0 & Appendix A v2.0 are lint-clean
    depends_on: [006.1, 006.2, 006.3]

deferred:
  - id: 001.9
    action: Diagram semantic drift → closure → action morphism
  - id: 004.6
    action: Begin Appendix or lineage sketches (paper 004)
  - id: 001.8-old
    action: Diagram semantic drift → closure → action morphism flow (superseded)

future:
  - id: 006.9
    action: Build PV tag search/index tooling (CLI-level)

open_questions:
  - qid: Q005.1
    text: Should §8 stay in the main document or move to a companion note?
  - qid: Q005.2
    text: Should surprise/anchoring metrics sit in PV5.x or PV3.x?
  - qid: Q005.3
    text: Would a SageMath-generated curvature-threshold heat-map be acceptable?
  - qid: 008.5
    text: Do we reserve “agent” only for bounded concernful systems?
  - qid: 009.6
    text: Representation of field morphisms for enriched categorical modelling?

---

#### 1. **Delete the source document**

- If the old action list was stored in an `.md`, `.yaml`, or `.json` file (e.g. `actions_2025-04-29.md`), delete it directly from Obsidian or your file system.
    
- Confirm you’re removing the one that included:
    
    > `id: 001 — Merge and track actions from 2025-04-29 Constraint Engine Report`
    

#### 2. **Remove from Obsidian links and backlinks**

- Use Obsidian’s **backlinks pane** or a vault-wide search (`[[actions_2025-04-29]]`) to remove or update all links to the trashed document.
    
- If embedded in higher-level dashboards or indexes, remove its `![[...]]` transclusion references.
    

#### 3. **Delete or archive obsolete queries**

- If the document was linked to Dataview queries (`TABLE`, `LIST`, `TASK` blocks), delete or archive those queries.
    
- You might grep for lines like:
    
    dataview
    
    CopyEdit
    
    `WHERE file.name = "actions_2025-04-29"`
    

#### 4. **Confirm metadata is not orphaned**

- If you were assigning custom frontmatter fields (e.g. `status:`, `source:`), confirm those aren’t skewing dashboards.
    
- Run a Dataview check:
    
    dataview
    
    CopyEdit
    
    `TABLE file.name, status, source WHERE status AND source SORT file.name ASC`
    

#### 5. **Repoint all canonical references to new list**

- Update internal planning notes, dashboards, or README-type docs to point to the **new board version** you’ve adopted (e.g. _UCSE / Theory-Stack Master Action Board — 2025-05-05_).
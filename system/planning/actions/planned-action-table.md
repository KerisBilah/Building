
|Action ID|Still marked ⟂|What would count as confirmation|Where I expect it to live|
|---|---|---|---|
|**001.1** UCSE Core Architecture sketch|`planned`|A diagram _or_ a top-level bullet list of modules (Morphism Stack, Constraint Cycle, Projection Mgr) with lines showing Rust coroutine boundaries.|`ucse/core/ucse_architecture.md` or a PNG/SVG in `/visual/`|
|**001.2** Fallacy-Selector Module design|`planned`|Section in _Constraint as Rhetoric_ (or a separate note) that lists fallacy classes, maps them to π-morphisms, and gives an interface stub.|`modules/fallacy_selector.md`|
|**001.4** Prolog-like traversal engine plan|`planned`|Design note showing grammar, back-tracking strategy, and an example query over 𝔽.|`ucse/trl/trl_backtracker.md`|
|**001.5** Library of field-analysis tools|`planned`|An index note with at least 3 operators beyond Voronoi (e.g. watershed, persistence, ridge-line) plus API signatures.|`ucse/analysis_tools/`|
|**001.6** Metric tracking spec|`planned`|Table or code snippet exposing curvature, contradiction, compressibility, relevance metrics at UCSE layer.|`ucse/metrics/ucse_metrics.md`|
|**001.8** Dual-space UCSE re-use proof|`active`|A short test or diagram showing the same module running on both 𝔽 and 𝔅 datasets.|`tests/dual_space_ucse.test.md`|
|**003.1–003.3** Geometric/topological operators & interfaces|`planned`|A note enumerating accepted operators, cost thresholds, and a Functor interface spec.|`ucse/geometric_ops/`|
|**004.1** _Before Belief_ — Introduction|`pending`|The first subsection of the paper (≈ 2-3 paragraphs) — even rough prose.|Inside `before_belief.md`|
|**004.4 / 004.7** Section 8 (philosophy/safety)|`planned`|Outline headings or bullet list of key arguments; doesn’t need full prose yet.|`before_belief.md`|
|**005.1–005.4 / 005.5** PV-schema hygiene tasks|`planned`|A commit diff or vault grep report showing updated YAML headers, inserted PV tags, and absence of (P1)… placeholders.|Git commit or Dataview query output|
|**006.1–006.4** Appendix A v2.0 build steps|`pending / blocked`|The actual `/spec/appendix-a_v2.yaml`, the moved diagram file, and a Lint/CI pass log.|`/spec/` and `/visual/`|
|**006.10 / 006.11** PV1.4 definition + mini-paper|`pending / planned`|New entry in Appendix A defining PV1.4 _and_ a stub note `pv/PV1.4.md` with abstract + dependencies.|`pv/` folder|
|**007.5** Vocabulary harmonisation pass|`in_progress`|A diff or note listing term replacements (“tensor-mode”, new closure labels) across MTOA and UCSE drafts.|`logs/harmonisation_2025-05-xx.md`|
|**007.6 / 007.9** $\mathcal{A}ct^{\dagger}$ operator|`pending / planned`|Formal definition in Appendix A **or** a section in _Agency as Causal Primitive v2.0_ with symbol, signature, and PV tag.|`appendix-a_v2.yaml` or `agency_causal_primitive_v2.md`|
|**007.10** Metric package (KAI, ρ_meta, etc.)|`planned`|A module file or Jupyter/Sage notebook bundling the metric functions, usage examples, and test vectors.|`metrics/package/`|
|**007.11** Field diagrams for γ, φ, τ|`planned`|Sketch PNG/SVGs or Markdown diagrams referenced in the paper.|`/visual/agent_fields/`|
|**008.1–008.5** Agent typology work|mixed|A glossary note plus tracked search-and-replace report for term harmonisation.|`glossary/agent_typology.md`|
|**009.1 / 009.2** Categories 𝔽 and 𝔅 definitions|`planned`|Two concise category blocks: objects, morphisms, identity, composition laws.|`category_theory/sem_categories.md`|

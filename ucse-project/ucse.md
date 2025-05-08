## ⬡ Project Name: ucse

## ⬡ Project Skeleton Structure

/ucse-project
├── /docs               # All human-readable specs and notes
│   ├── foundational-priors.md
│   ├── modular-epistemology.md
│   ├── infrastructure-plan.md
│   ├── ucse-spec.md
│   └── ...
├── /src                # Source code by major module
│   ├── /ucse-engine
│   ├── /tensor-ops
│   ├── /constraint-layer
│   ├── /scaffold-system
│   ├── /visualization
├── /middleware         # Middleware components (if separated)
│   ├── reflex_scanner/
│   ├── closure_monitor/
│   ├── tranche_scheduler/
├── /tests              # Unit and integration tests
├── /visual             # Static visual artefacts, Mermaid, SageMath diagrams
├── /logs               # MVTs, scaffold traces, provenance logs
│   ├── /meta_logs      # Reflex metadata, authorship mode, AI trace info
└── README.md

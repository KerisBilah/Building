## ⬡ Project Name: IntentWeave

> IntentWeave is a lightweight, trace-aware middleware for expressing, combining, and projecting test intentions in semantically coherent engineering systems.

The name reflects:

- _intent_ (engineering purpose, tied to belief traceability),    
- _weaving_ (composability, design layering, constraint architecture),
- and the architecture’s focus on semantic traceability.

## ⬡ Project Skeleton Structure

This assumes we are starting with a Rust implementation, with SageMath and Markdown support for analysis and design interface.

intentweave/
├── Cargo.toml                                     # Rust project config
├── README.md                                  # Project overview and schema definitions
├── src/
│   ├── lib.rs                                            # Core types and logic
│   ├── schema/
│   │   ├── mod.rs                                     # Intent schema declarations
│   │   ├── test_intent.rs                           # TestIntent struct, validation logic
│   │   └── idioms.rs                                 # Composable intent idioms
│   ├── evaluation/
│   │   ├── mod.rs                                    # Evaluation surface (proj. logic)
│   │   └── collapse.rs                              # Collapse trigger (∇ΔΞ > θ)
│   ├── storage/
│   │   ├── mod.rs                                    # Trace and log handling
│   │   └── tau_trace.rs                             # Write and version τ_D
│   └── utils/
│       └── math_helpers.rs                      # Tensor and vector ops
├── tests/
│   ├── intent_tests.rs                             # Unit tests for schema and idioms
│   └── collapse_tests.rs                         # Projection + trace write tests
├── design/
│   ├── schema-examples.md                # Expressive test idioms
│   └── theory-links.md                          # Linkage to MTBT, METED, PV structure
├── visual/
│   └── intent_space.sage                      # SageMath visualisations
└── docs/
    └── design-intent-guide.md         # For engineers using the dashboard


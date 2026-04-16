# FARD WIN DEMO

FARD WIN DEMO is a single-repo adoption demo designed to prove, with real receipts and replayable outputs, that FARD can solve the most painful day-to-day problems faced by three incumbent cohorts:

- Python users: dataframes, ML checkpoints, heavy deploy stacks
- Rust users: startup time, concurrency ceremony, systems-style throughput
- JavaScript users: full-stack drift, package chaos, supply-chain instability

This repo is organized around four runnable demo experiences:

- `apps/py_pain_demo` — analytics, plotting, checkpointed model training, and serving
- `apps/rust_pain_demo` — startup measurement, parallel pipelines, JSON throughput
- `apps/js_pain_demo` — typed full-stack demo, digest-pinned packages, request tracing
- `apps/control_tower` — receipts, replay verification, benchmark collection, report rendering

## What this repository is

This repository is a **build-ready specification pack** for implementing the full demo in VS Code. It includes:

- the exact repo layout
- exhaustive README and build instructions
- VS Code workspace settings and tasks
- package-by-package contracts
- benchmark targets and acceptance criteria
- data requirements
- delivery sequencing
- artifact and report formats

It does **not** pretend to be a finished executable implementation when the underlying FARD runtime, stdlib names, AOT surface, HTTP server surface, and package registry APIs are not yet fully fixed. The point of this repo is to remove planning ambiguity so implementation can begin immediately.

## Why this demo exists

People do not adopt new languages because they are elegant. They adopt when the pain of staying is worse than the pain of switching, when the new tool solves a problem they actually have, and when the migration path is gradual.

This demo is built to prove all three.

## Demo goals

### Python cohort
Show:

- DataFrame-style analytics pipeline
- plot generation
- small ML training run with checkpoint CIDs
- one-command local serving
- full receipt chain across the pipeline

### Rust cohort
Show:

- tiny startup cost
- real parallel map/filter/reduce flow
- JSON throughput measurements
- benchmark report with digest-backed outputs
- receipt chain across all benchmark stages

### JavaScript cohort
Show:

- typed full-stack flow
- shared contracts between backend and frontend
- digest-pinned package manifest
- request trace receipt
- reproducible bundle/build artifact

### Control tower
Show:

- all receipts collected
- replay verification pass/fail
- benchmark table generated
- summary report rendered to JSON and Markdown

## Repository layout

```text
FARD WIN DEMO/
  .vscode/
  apps/
    py_pain_demo/
    rust_pain_demo/
    js_pain_demo/
    control_tower/
  packages/
    receipt-core/
    replay-core/
    report-core/
    bench-core/
    dataframe-core/
    plot-core/
    ml-core/
    serve-core/
    par-core/
    json-core/
    web-core/
    dom-core/
    type-share-core/
    install-core/
  docs/
  data/
  out/
  fard.toml
```

## Build philosophy

No fake wins.

Every benchmark, receipt, replay check, plot, and comparison must be produced by actual FARD execution. There are no placeholder benchmark numbers, no mocked receipt digests, no “simulated” package installs.

Where infrastructure is missing, implementation work must land before the demo claim is made.

## The four demos

### 1. Python pain demo

Input:
- `sales_10m.csv`
- `events_1m.jsonl`

Output:
- grouped aggregations
- sorted summaries
- plot artifact
- model checkpoints by CID
- served result endpoint
- receipts for each stage

Claim:
FARD replaces a meaningful slice of Pandas + plotting + ML checkpointing + lightweight API serving.

### 2. Rust pain demo

Input:
- `payload_10mb.json`
- a large numeric array or generated range

Output:
- startup timing
- JSON parse timing
- parallel pipeline timing
- optional FFI timing if available and policy-safe
- receipts for all measured stages

Claim:
FARD delivers systems-style practicality with less ceremony.

### 3. JS pain demo

Input:
- shared type definitions
- package manifest
- seeded user records

Output:
- backend API artifact
- frontend render/bundle artifact
- shared types imported on both sides
- digest-pinned install manifest
- request trace receipt

Claim:
FARD removes frontend/backend drift and package instability.

### 4. Control tower

Input:
- outputs from all three demos

Output:
- `summary.json`
- `summary.md`
- `benchmark_table.json`
- `replay_checks.json`
- collected receipt directory

Claim:
Every reported win is measurable, digested, and replay-verified.

## Build order

1. `receipt-core`
2. `replay-core`
3. `report-core`
4. `bench-core`
5. `dataframe-core`
6. `plot-core`
7. `ml-core`
8. `serve-core`
9. `par-core`
10. `json-core`
11. `web-core`
12. `type-share-core`
13. `install-core`
14. `dom-core`
15. `apps/py_pain_demo`
16. `apps/rust_pain_demo`
17. `apps/js_pain_demo`
18. `apps/control_tower`

## VS Code workflow

Open the root folder in VS Code.

Recommended sequence:
1. Read `docs/ARCHITECTURE.md`
2. Read `docs/PACKAGE_CONTRACTS.md`
3. Read `docs/BUILD_ORDER.md`
4. Start with `packages/receipt-core`
5. Implement package-by-package
6. Wire each app only after its dependencies are real
7. Run control tower last

## What success looks like

A skeptical developer runs one command per cohort and says:

- Python: “This actually solves analytics + reproducibility.”
- Rust: “This is readable, fast, and measured.”
- JS: “This removes full-stack drift and package instability.”

## Artifact outputs

The demo must eventually emit:

```text
out/
  py_demo/
  rust_demo/
  js_demo/
  control_tower/
```

Each directory must contain:
- machine-readable results
- human-readable summary
- receipts
- replay verification material where applicable

## Current status

This repo is prepared for implementation in VS Code and zipped as a delivery artifact. It is comprehensive on architecture and contracts. The code-level implementation must still be completed against the exact FARD runtime and stdlib available in your environment.

See:
- `docs/ARCHITECTURE.md`
- `docs/PACKAGE_CONTRACTS.md`
- `docs/BENCHMARKS.md`
- `docs/IMPLEMENTATION_PLAN.md`

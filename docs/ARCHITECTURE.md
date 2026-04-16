# Architecture

## Top-level principle

The demo is not a marketing page. It is a measurable execution system with four outputs:
1. Python cohort win
2. Rust cohort win
3. JavaScript cohort win
4. control tower proof layer

## Shared invariants

Every major stage must produce:
- a machine-readable result
- a human-readable summary
- a receipt or receipt chain
- a digest of the output artifact
- a replay verification input if the stage is replayable

## Repo layers

### `packages/`
Reusable implementation units.

### `apps/`
Cohort-facing demo experiences.

### `docs/`
Contracts, build order, targets, and implementation sequencing.

### `data/`
Benchmark and seed data.

### `out/`
Execution artifacts.

## Cohort separation

### Python
Focus on dataflow and deploy simplicity.

### Rust
Focus on startup, throughput, parallelism, and simplicity.

### JS
Focus on full-stack coherence, package determinism, and shared contracts.

## Control tower
This is the truth layer. Any claim not represented in control tower output does not count.

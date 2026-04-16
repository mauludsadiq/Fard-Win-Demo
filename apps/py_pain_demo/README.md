# Python Pain Demo

## Goal
Demonstrate:
- DataFrame ingest and analytics
- plot artifact generation
- small-model training with checkpoint digests
- local serving
- full receipt capture

## Expected outputs
- `summary.json`
- `summary.md`
- `receipts/`
- `plots/`
- `checkpoints/`

## Required packages
- `dataframe-core`
- `plot-core`
- `ml-core`
- `serve-core`
- `receipt-core`
- `replay-core`
- `report-core`

## Acceptance criteria
- analytics result is deterministic
- plot artifact has digest
- checkpoint digests are emitted per epoch or save point
- local endpoint serves result output

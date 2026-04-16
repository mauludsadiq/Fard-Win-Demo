# Rust Pain Demo

## Goal
Demonstrate:
- startup measurement
- JSON parse throughput
- parallel map/filter/reduce
- receipt-backed benchmark output

## Expected outputs
- `startup.json`
- `json_bench.json`
- `parallel_bench.json`
- `summary.md`
- `receipts/`

## Required packages
- `bench-core`
- `par-core`
- `json-core`
- `receipt-core`
- `report-core`

## Acceptance criteria
- startup measurement is captured
- JSON payload digest is recorded
- parallel reduction result is deterministic
- all benchmark stages emit receipts

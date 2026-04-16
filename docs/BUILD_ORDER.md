# Build Order

## Phase 1 — Proof primitives
1. `receipt-core`
2. `replay-core`
3. `report-core`
4. `bench-core`

## Phase 2 — Python win
5. `dataframe-core`
6. `plot-core`
7. `ml-core`
8. `serve-core`

## Phase 3 — Rust win
9. `par-core`
10. `json-core`

## Phase 4 — JS win
11. `web-core`
12. `type-share-core`
13. `install-core`
14. `dom-core`

## Phase 5 — App integration
15. `apps/py_pain_demo`
16. `apps/rust_pain_demo`
17. `apps/js_pain_demo`
18. `apps/control_tower`

## Rule
No app code should depend on a package that has not already been made real.

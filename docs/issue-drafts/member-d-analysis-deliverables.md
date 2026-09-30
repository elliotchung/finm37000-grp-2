# Draft Issues — Member D (Analysis & Deliverables)

## D1. Core analysis / model
- **Goal:** Implement the main computation in `src/finm37000_grp2/analysis.py`, taking the clean data from C3 as input.
- **Acceptance criteria:** A pure function with a clear signature and docstring, plus unit tests on synthetic data.
- **Blocked by:** C3 (schema only; can start with synthetic data)
- **Labels:** `analysis`

## D2. Evaluation and sanity checks
- **Goal:** Metrics or checks that show the results are correct and meaningful, such as benchmarks, known values, or robustness checks.
- **Acceptance criteria:** Tests or a notebook that compares the results against a reference.
- **Blocked by:** D1
- **Labels:** `analysis`

## D3. Visualization and reporting
- **Goal:** Produce the figures and tables that communicate the result.
- **Acceptance criteria:** A script or notebook that regenerates all outputs into `reports/` from a single command.
- **Blocked by:** D1
- **Labels:** `analysis`, `docs`

## D4. Final deliverable and documentation
- **Goal:** Wire everything into the entry point and update the README "How to Run" section so that it is accurate.
- **Acceptance criteria:** A fresh clone followed by `uv sync && uv run python -m finm37000_grp2` reproduces the results.
- **Blocked by:** C4, D3
- **Labels:** `docs`

# Draft Issues — Member C (Data & Infrastructure)

## C1. Identify and document data sources
- **Goal:** Decide exactly which data the project needs and where it comes from.
- **Acceptance criteria:** README "Data" section lists the sources, fields, frequency, date range, and access method. Any API keys are documented in `.env.example` (never committed).
- **Labels:** `data`, `docs`

## C2. Implement data loader
- **Goal:** A function `load_raw(...)` in `src/finm37000_grp2/data.py` that downloads or reads raw data into `data/raw/`.
- **Acceptance criteria:** Idempotent (skips if cached), with a unit test that uses a small fixture.
- **Blocked by:** C1
- **Labels:** `data`

## C3. Clean and validate data
- **Goal:** `clean(raw) -> DataFrame` that handles missing values, types, timezones, and duplicates.
- **Acceptance criteria:** Documented output schema (column names and dtypes), with tests for the edge cases.
- **Blocked by:** C2
- **Labels:** `data`

## C4. Configuration and reproducibility
- **Goal:** Central config (paths, date ranges, tickers/symbols) and a one-command pipeline run.
- **Acceptance criteria:** `uv run python -m finm37000_grp2` runs end-to-end on the sample data, and CI passes.
- **Labels:** `infra`

## Interface (agree with Member D)
Write down the clean-data schema that Member D's analysis will consume, either in C3 or in a separate issue.

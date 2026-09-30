# FINM 37000 — Group 2 Project

> **Status: skeleton.** This README is a placeholder created by the Tech Lead.
> The **Communication Lead** will replace the sections marked `TODO` in a
> Pull Request from their fork (see [docs/roles.md](docs/roles.md)). Every team
> member must review and approve that PR before it is merged.

## Project Goal

TODO (Communication Lead): In 2–4 sentences, describe the analysis or
application the team agreed to build, who it is for, and what question it
answers.

## Desired Outcome

TODO (Communication Lead): Describe the concrete deliverables, such as a report,
a CLI, a dashboard, or a notebook, and what "done" looks like.

- [ ] Deliverable 1
- [ ] Deliverable 2
- [ ] Deliverable 3

## Data

TODO: What data sources will be used, how they are obtained, and any access
requirements (API keys, licenses). Raw data is **not** committed; it goes in
`data/`, which is git-ignored.

## How to Run

The project uses [uv](https://docs.astral.sh/uv/) for environment management.

```bash
# 1. Clone your fork
git clone https://github.com/<your-username>/finm37000-grp-2.git
cd finm37000-grp-2

# 2. Create the environment and install dependencies
uv sync

# 3. Run the tests
uv run pytest

# 4. Run the project (aspirational — update once the entry point exists)
uv run python -m finm37000_grp2
```

## Repository Layout

```
.
├── src/finm37000_grp2/   # Project Python package
├── tests/                # pytest tests
├── notebooks/            # Exploratory notebooks
├── data/                 # Local data (git-ignored)
├── docs/                 # Assignment docs, roles, and planning notes
└── .github/              # Issue/PR templates and CI
```

## Roadmap

The work is tracked as GitHub Issues. See the
[open issues](../../issues) for the task breakdown and who owns each task.

## Team

See [docs/roles.md](docs/roles.md) for role assignments and responsibilities,
and [CONTRIBUTING.md](CONTRIBUTING.md) for the Git/GitHub workflow.

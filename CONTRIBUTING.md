# Contributing

## Workflow (fork & pull request)

The Tech Lead's repository is the **main** repo. Everyone else works on a fork.

```bash
# One-time setup
gh repo fork <tech-lead>/finm37000-grp-2 --clone
cd finm37000-grp-2
git remote -v   # origin = your fork, upstream = main repo

# For each task
git fetch upstream
git switch -c <short-branch-name> upstream/main
# ...make changes...
uv run ruff check . && uv run pytest
git push -u origin <short-branch-name>
gh pr create --repo <tech-lead>/finm37000-grp-2
```

## Rules

- Do not push directly to `main`. All changes go through a PR.
- Link the issue that the PR addresses in the PR description (for example, `Closes #12`).
- Each PR needs **at least one approving review** from a teammate. The README
  PR in Part 1 needs approval from **all four members**.
- Keep PRs small and focused on one issue.
- Put discussion on GitHub (PR and issue comments) rather than only in chat,
  because contributions are graded on what is visible in the repository.

## Development

```bash
uv sync                 # install dependencies
uv run pytest           # run tests
uv run ruff check .     # lint
uv run ruff format .    # format
uv add <package>        # add a dependency (commits pyproject.toml + uv.lock)
```

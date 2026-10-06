# Roles & Responsibilities — Project Part 1

Placeholder names are used below. Replace `Member A`–`Member D` with real names
and GitHub handles once roles are agreed.

| Placeholder | Name | GitHub | Part 1 Role |
|-------------|------|--------|-------------|
| Member A | Elliot Chung | @elliotchung | Tech Lead |
| Member B | Vidhi Jain | @vidhijain28 | Communication Lead |
| Member C | Divyaa Dehlan | @dehlandivya | Design Lead — Data & Infrastructure |
| Member D | Kayla Hammonds | @khammonds530-max | Design Lead — Analysis & Deliverables |

Roles apply to Part 1 only, except that **the Tech Lead owns the main
repository for the whole course** and is the gatekeeper for merging PRs.

## Equal-Contribution Principle

The rubric grades each member on three things:

1. **Completed Delegated Task** (5 pts): your own role's deliverable.
2. **Contributed to README** (5 pts): reviewing and approving the README PR.
3. **Contributed to Issue Roadmap** (10 pts): writing issues and commenting on them.

To make contributions equal and **visible on GitHub**, every member has:

- one **delegated deliverable** of about the same size (below), and
- the same **non-delegated duties** (see [Shared Duties](#shared-duties-everyone)).

---

## Member A — Tech Lead

**Delegated deliverable:** a working starting repository shared with the team.

- [ ] Create the GitHub repo under their account and push the project skeleton
      (package layout, `pyproject.toml`, tests, CI, templates).
- [ ] Add Members B, C, and D as collaborators, or confirm they have forked.
- [ ] Set branch protection on `main` so changes require a PR and at least one approval.
- [ ] Create issue labels (`data`, `analysis`, `infra`, `documentation`, `part-1`).
- [ ] Post the repo link on the team channel, and confirm each member has forked and cloned it.
- [ ] Merge the README PR once **all four** members have approved it.

## Member B — Communication Lead

**Delegated deliverable:** the README PR describing the agreed plan.

- [ ] Fork the repo and create a branch named `readme-plan`.
- [ ] Fill in every `TODO` section of `README.md`: Project Goal,
      Desired Outcome, Data, How to Run (aspirational), and Team.
- [ ] Open a PR from `readme-plan` into the Tech Lead's `main`, using the PR template.
- [ ] Reply to all review comments and push revisions until everyone approves.
- [ ] Make sure the README links to the issue roadmap once issues exist.

## Member C — Design Lead (Data & Infrastructure)

**Delegated deliverable:** the issues covering the **first half** of the
project pipeline, from getting the data to having clean, usable data.

- [ ] Open about 4 issues using the "Task" issue template, covering data
      sourcing, ingestion/loading, cleaning/validation, and storage/config.
- [ ] Give each issue a goal, acceptance criteria, dependencies, and a suggested owner.
- [ ] Label the issues `data` or `infra`, and link dependencies (for example, "blocked by #N").
- [ ] Coordinate with Member D so that the interface between the two halves
      (the clean dataset schema or function signature) is written down in an issue.

## Member D — Design Lead (Analysis & Deliverables)

**Delegated deliverable:** the issues covering the **second half** of the
project pipeline, from clean data to the final deliverable.

- [ ] Open about 4 issues using the "Task" issue template, covering the core
      analysis/model, evaluation/testing, visualization/reporting, and the
      final entry point/documentation.
- [ ] Give each issue a goal, acceptance criteria, dependencies, and a suggested owner.
- [ ] Label the issues `analysis` or `documentation`, and link dependencies on Member C's issues.
- [ ] Make sure that completing all the issues leads to the outcome described in the README.

> Draft issue outlines for Members C and D are in
> [docs/issue-drafts/](issue-drafts/). They are **starting points only**. Each
> Design Lead should rewrite them for the chosen topic and open them on GitHub
> under their own account.

---

## Shared Duties (Everyone)

These are required of **all four members**, and each should leave a visible
trace on GitHub:

- [ ] **Fork** the main repo.
- [ ] **Review the README PR**: leave at least one substantive comment or
      suggestion, then submit an **Approve** review when satisfied.
- [ ] **Review the issue roadmap**: comment on **at least 2 issues you did
      not write**, for example on scope, missing acceptance criteria,
      dependencies, or an offer to own the task. React 👍 to issues you agree with.
- [ ] If there is a gap in the roadmap, **open a new issue** or suggest one in a comment.
- [ ] Self-assign or volunteer for at least 2 implementation issues so that the
      later implementation work is spread evenly (about 2 issues per person).

## Communication

- **Primary channel:** TODO (for example Slack, iMessage group, or email)
- **GitHub notifications:** each member should "Watch → All Activity" on the
  main repo and confirm in the team channel that notifications are arriving.
- **Expected response time on PRs/issues:** TODO (for example, within 24 hours)

## Part 1 Timeline

| Step | Owner | Target date |
|------|-------|-------------|
| Repo created and shared | Member A | TODO |
| All members forked | Everyone | TODO |
| README PR opened | Member B | TODO |
| Issues opened | Members C & D | TODO |
| README PR reviewed and approved | Everyone | TODO |
| Issue comments and revisions | Everyone | TODO |
| README merged, repo link submitted | Member A | TODO |

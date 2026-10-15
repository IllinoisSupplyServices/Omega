# Verification standard

**Produced is not verified.** A file, PR, command invocation, or agent claim proves only what its evidence supports. Every work item ends with one explicit outcome and evidence.

## Check before acting

Before creating or changing anything, inspect the relevant existing files, task history, branches, PRs, and available verification evidence. Confirm the current state and authority of relevant sources. Reuse or extend existing work so work is never duplicated. If access is unavailable, report that limit rather than assuming the work does not exist.

Keep department records in Google Drive's authoritative Fresh Start folder. Repository changes contain engineering artifacts and pointers, never copies of department records.

## Verification process

1. Compare the assignment with the actual diff and produced artifacts. Check scope, required files, links, and stated system boundaries.
2. Run the checks appropriate to the repository's current contents. Record the exact command or workflow, commit or PR, result, and useful output or evidence link.
3. Exercise relevant failure cases for new checks so success is meaningful.
4. Separate observations from assumptions. State checks not run, unavailable access, dependencies, failures, and remaining risks.
5. Have a Verifier review the artifacts and evidence against the assignment. Builder self-checks support this review; they do not replace it.
6. Report the terminal outcome below. Nothing merges unreviewed; opening a PR or passing automation is not merge approval.

## Terminal outcomes

| Outcome | Meaning and required evidence |
| --- | --- |
| COMPLETE | All assigned deliverables and applicable verification criteria are satisfied. Link the artifacts and passing checks; identify the Verifier's review evidence where required. |
| COMPLETE_WITH_EXCEPTIONS | Deliverables are produced, with explicit verification or acceptance exceptions. Provide evidence for completed checks and name each exception, its impact, and follow-up. Do not present this as full verification. |
| BLOCKED | A dependency, access limit, or missing decision prevents required progress or verification. Show the blocker, attempted checks, completed work, and what would unblock it. |
| FAILED | An attempted action or check failed against the criteria. Provide the failing command or action, observed result, affected scope, and remaining work. |
| ABORTED | Work stopped intentionally before completion. State why, the last confirmed state, partial artifacts, and any cleanup or handoff needed. |

Use one outcome for the work item; individual checks may have different results. A useful report includes: outcome, artifact/PR and commit, expected versus observed results, commands or workflow links, review evidence, and exceptions or next steps. Never label unrun checks as passing.

## Current automated checks

[The verify workflow](../.github/workflows/verify.yml) runs on pull requests and checks:

- Required files exist: README.md, AGENTS.md, docs/SYSTEM_MAP.md, and docs/VERIFY.md.
- Every tracked Markdown file (case-insensitive .md extension) contains non-whitespace content.

Missing required files or empty Markdown fail the job. These are structural documentation checks only. They do not establish correctness of prose, working external links, Drive access, application behavior, or Verifier approval. No application test suite is currently defined, so application tests cannot be run.

Return to [Start Here](../README.md).

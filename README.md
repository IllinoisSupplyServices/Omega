# Omega — Start Here

Omega is the engineering home of **Fresh Start (Illinois Supply & Services)**.

## Authority rule

Google Drive's **Fresh Start** folder is the authoritative workspace. This repository holds engineering artifacts and pointers, never copies of department records. Consult the authoritative Drive record before acting; keep records and their updates in Drive.

No verified Fresh Start folder URL exists in the current repository. Obtain the authorized folder link before accessing records; do not guess a destination or create a replacement workspace.

## Find your starting point

| Need | Start here |
| --- | --- |
| Department records and business source material | Google Drive's Fresh Start folder (authoritative workspace) |
| System boundaries and handoffs | [System map](docs/SYSTEM_MAP.md) |
| Agent repository instructions | [AGENTS.md](AGENTS.md) |
| Evidence, checks, and outcome reporting | [Verification standard](docs/VERIFY.md) |
| Automated scaffold checks | [verify workflow](.github/workflows/verify.yml) |

## Three-system map

- **Google Drive = records authority.** Fresh Start's authoritative workspace and department records live here.
- **GitHub = engineering control plane.** Omega holds engineering documentation, code when introduced, task discussions, pull requests, review, and check evidence.
- **Codex Cloud = coding agent environments bound to these repositories.** Agents inspect a repository, carry out scoped engineering tasks, and propose changes through PRs.

See [SYSTEM_MAP.md](docs/SYSTEM_MAP.md) for the topology and boundaries.

## How work flows

1. Check existing files, tasks, branches, PRs, and available verification evidence before acting so work is never duplicated.
2. Read the relevant repository instructions and consult authoritative Drive records when needed.
3. Codex tasks produce focused PRs with a file summary, checks, evidence, and explicit limitations.
4. A Verifier reviews the diff and evidence against the assignment. Producing an artifact is not verification.
5. Nothing merges unreviewed. Checks support review; they do not authorize a merge.

This is a documentation-stage repository. The verify workflow checks required files and non-empty Markdown; it does not validate business records, application behavior, or review approval.

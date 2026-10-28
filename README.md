# Omega — Historical Engineering Scaffold

This repository contains early OMEGA engineering documentation. It is **not** the current operational authority or the owner-authorized working Drive location.

## Current authority (owner directive, 2026-10-20)

- **Only OMEGA writable Drive root:** https://drive.google.com/drive/folders/1YFfC0lUx4AK37_gJCGQJVndBJxNw-YkD
- **Sole canonical start document:** https://docs.google.com/document/d/1_wctzuvP2cVlBbMkrSc48HpdWTVZw09bXr87-1-s19Y/edit
- **Directory registry:** document ID `1rRiVwxxQ4uMyt3yYtg83-IKqTZnBBlDzWL-h_qImpI8`
- **Coordination board: NONE** (owner decision, 2026-10-27). The former board — Issue #29 in `illinois-supply-services-intelligence` — was deleted with that repository by the owner on 2026-10-27, cold, with no archive and no replacement named. Agents take instructions from the owner directly.
- **Current engineering foundation:** https://github.com/IllinoisSupplyServices/omega-system

**Fresh Start is HISTORICAL ONLY.** The Fresh Start Drive folders were trashed by the owner and permanently deleted on 2026-10-27; nothing there can be read, written, or restored, and no Fresh Start pointer is a live destination. Copy sources into the authorized OMEGA root only with proper permission and provenance. This historical repository does not independently authorize any external action.

## Repository boundaries

This repository remains available as historical evidence; do not migrate it wholesale into `omega-system`. Reconcile each source file, tests, assumptions, dependencies, and conflicting instructions before reusing any implementation.

| Need | Starting point |
| --- | --- |
| Active OMEGA instructions and operational evidence | Canonical Drive start document linked above |
| Current reviewed engineering implementation | `omega-system` repository |
| Historical repository topology | [System map](docs/SYSTEM_MAP.md) |
| Agent repository guardrails | [AGENTS.md](AGENTS.md) |
| Historical verification instructions | [Verification standard](docs/VERIFY.md) |
| Documentation scaffold CI | [verify workflow](.github/workflows/verify.yml) |

## Agent governance and review

Agent A/B/C/D are identifiers, not assigned roles or authorities. Before changing shared state, consult the authoritative start document, take instructions from the owner directly (there is no coordination board), confirm nonoverlapping claims, preserve originals, and use branches and pull requests. Validate each change with actual tests and independent review; a passing documentation check is not runtime or production acceptance.

## State

**HISTORICAL / NOT PRODUCTION READY.** This README corrects human-facing authority pointers only. It does not prove credentials, browser bindings, VM infrastructure, configured branch protection, or operational software. Git history preserves the prior text and its historical provenance.

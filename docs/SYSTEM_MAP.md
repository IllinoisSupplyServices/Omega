# System map

Omega is the engineering home of Fresh Start (Illinois Supply & Services). Three systems have distinct responsibilities.

## Topology

```text
Google Drive: Fresh Start folder
  authoritative workspace / department records
            |
            | authorized source consultation and pointers
            v
GitHub: Omega
  engineering artifacts / tasks / branches / PRs / review / checks
            ^
            | repository context in; proposed changes and evidence out
            |
Codex Cloud
  coding agent environments bound to these repositories
```

This describes the working model, not proof of configured integrations or access.

## Google Drive — records authority

The Fresh Start folder in Google Drive is the authoritative workspace. Department records remain there. Omega may hold pointers to those records and engineering artifacts needed to build or maintain systems; it must never hold copies of department records.

Consult the current authoritative source before work that depends on it. A repository pointer does not grant access or replace the record. No verified Drive folder URL is present in the repository; obtain the authorized pointer rather than inventing one. Do not create a parallel records workspace.

## GitHub — engineering control plane

Omega contains engineering artifacts and pointers. GitHub provides the proposed-change boundary: tasks lead to branches and PRs, checks supply limited evidence, and a Verifier reviews the resulting diff and evidence. Nothing merges unreviewed.

At scaffold time, the base repository contains a README; the existing agent-instructions PR supplies AGENTS.md. This scaffold adds system and verification documentation plus a documentation check. There is no application, dependency manifest, or application test suite to claim as validated.

## Codex Cloud — coding environments

Codex Cloud provides coding agent environments bound to these repositories. An agent reads repository instructions and existing work, makes only authorized changes, runs available checks, and produces a PR with evidence. An environment is an execution workspace, not the authority for department records or an approval to merge.

Environment bindings, credentials, Drive access, and branch protection must be confirmed through their actual configuration when needed; this document does not establish that they are configured.

## Handoffs and boundaries

1. Check existing work and evidence before acting. Reuse or extend the appropriate work instead of duplicating it.
2. Consult Drive for authoritative business context, retaining only appropriate pointers in engineering artifacts.
3. Perform engineering work in the repository through a Codex task and branch.
4. Submit a PR describing the change, validation, exceptions, and dependencies.
5. A Verifier inspects scope and evidence under [VERIFY.md](VERIFY.md). Corrections return to the PR.
6. Merge only after review and applicable checks. Documentation alone does not enforce this rule; no repository settings are changed by this scaffold.

Return to [Start Here](../README.md).

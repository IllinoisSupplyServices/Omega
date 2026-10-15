# Agent instructions

## Project
- The repository is named Omega in `README.md`. That file contains only the heading `# Omega`.
- No application code is present; the project's purpose and behavior are not documented.

## Setup
- No dependency manifests, installation commands, environment configuration, or setup instructions are present. There is no documented dependency installation or environment preparation procedure.

## Tests and checks
- No tests, test runner, lint configuration, CI workflows, or governance checks are present. There are no repository-defined commands for running them.
- Before finishing work, run the full test suite if one is available. Report the exact command and result honestly, including failures. If no suite exists, explicitly report that tests could not be run because none is defined.

## Observable conventions
- The existing content is a root-level `README.md` using a Markdown ATX heading.
- No source layout, code naming, formatting, or language conventions can be inferred from the current repository.

## Guardrails
- Never commit secrets, credentials, or tokens.
- Never weaken or edit tests just to make them pass; fix the underlying code.
- Keep changes minimal and focused on the task.
- Ground repository guidance in files that actually exist; do not invent tools, commands, or structure.

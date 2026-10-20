# ADR-0001: Local-first development with public GitHub history

Status: Accepted

## Decision
Use VS Code and local Git for development. Publish reviewed commits to a public GitHub repository. The repository is the canonical source of code, tasks and documentation.

## Consequences
- No dependence on GitHub Actions for local builds.
- Public commits must not contain credentials or sensitive captures.
- The assistant reads published repository state when provided with its URL; no assumed automatic synchronization.

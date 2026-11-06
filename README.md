# BellLabs Agentic SDLC

The upstream of the BellLabs documentation and lifecycle toolchain: the `sdlc` CLI, the skills,
the git hook templates, the GitHub workflow template, and the owner's ideas workspace. No
repository depends on this one at runtime; each vendors a pinned copy under `.sdlc/` and
`.agents/skills/` (see `docs/README.md`).

Program of record: `platform/mission-control/docs/specs/agentic-sdlc-2026-11/` (SPEC-01, PR-01,
DOC-01, the answers of sitting I). Decisions: Mission Control ADR-0064 to ADR-0067.

| Directory | Holds |
| --- | --- |
| `ideas/` | the owner's ideas workspace; read `ideas/README.md` before picking one up |
| `tools/` | the CLI source and its tests (slice S1, not yet present) |
| `skills/` | the skills published to repositories with `npx skills add jbell-rusty-vantage/agentic-sdlc`; first: `sdlc-docs` (navigate, update, truth pass) |
| `templates/` | hook scripts and `sdlc.yml` (slice S1) |
| `docs/` | the contract and the pointer to the program |

Workspace path: `BellLabs/platform/agentic-sdlc`. Remote: public [`jbell-rusty-vantage/agentic-sdlc`](https://github.com/jbell-rusty-vantage/agentic-sdlc), `main` only; history
starts at the 2026-11-06 clean-slate baseline ([repository history](docs/REPOSITORY-HISTORY.md)).

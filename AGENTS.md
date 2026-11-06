# belllabs-agentic-sdlc

This repository is the upstream of the BellLabs SDLC toolchain and the owner's ideas workspace. It
is not a runtime dependency of any other repository: never add an import, a path or a hook in
another repository that reaches here. Changes to the CLI, skills or templates are released and
pulled into repositories by decision (`sdlc update`).

- Ideas: `ideas/` (guide in `ideas/README.md`). Agents pick up `status: seed` ideas, set
  `status: interviewing`, cite the `ID-n`, and never edit the owner's itch paragraph.
- The specification: `../mission-control/docs/specs/agentic-sdlc-2026-11/SPEC-01-AGENTIC-SDLC.md`.
- The next session before implementation is the navigation-quality session named there (§12).
- Startup delivery mode and the owner reporting directive of `BellLabs/AGENTS.md` apply.
- No secrets, no runtime receipts, no personal notes in this repository.

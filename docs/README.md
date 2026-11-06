# The contract, in one page

Every BellLabs repository carries the same documentation contract, enforced by the vendored CLI
(`.sdlc/cli.mjs`). The contract is specified in Mission Control's
`docs/specs/agentic-sdlc-2026-11/SPEC-01-AGENTIC-SDLC.md` §3; this page will carry the extracted
rules once the CLI exists (slice S1), so that a repository never needs the program to read them.

Pinning: `.sdlc/lock.json` (CLI version, commit, digests) and `skills-lock.json` (skills).
Pulling: `node .sdlc/cli.mjs update --to <version>`; `npx skills add Overton77/belllabs-agentic-sdlc`.

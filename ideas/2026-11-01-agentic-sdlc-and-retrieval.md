---
id: ID-1
title: Agentic SDLC and retrieval quality across the BellLabs codebases
status: specified
domains: [mission-control, knowledge-services, aiengineer, biotech, agentic-sdlc]
created: 2026-11-01
owner: owner
promoted_to: platform/mission-control/docs/specs/agentic-sdlc-2026-11 (answers/AGENTIC-SDLC-SITTING-I-2026-11-01-ANSWERS.md)
linear: OVE-205 (parent), OVE-206..OVE-214 (slices)
---

# Agentic SDLC and retrieval quality across the BellLabs codebases

## The itch

We need automated documentation updates that respond to commit history and work. We are in a
start up stage so we are moving fast and breaking things, proverbially but we need to have some
fundamental parts of the SDLC baked in AT THE AGENTIC LEVEL. The hooks have to be intertwined with
git lifecycle of this codebase not scheduled. Agents being able to navigate these codebases might
be the most critical thing we build.

## The outcome

Every repository passes the same documentation checks, retrieval fixtures and drift gates from
git hooks and pull request jobs; an agent finds the current fact in one or two hops; ideas,
interviews, specs, issues and commits form one traceable chain.

## Where it lives

`platform/agentic-sdlc` (upstream), vendored into every repository.

## Constraints

Owner subscriptions (Cursor first), no scheduler, no runtime dependency on the upstream, startup
delivery mode.

## Evidence

Sitting I answers AS-D1 to AS-D20; Mission Control ADR-0064 to ADR-0067; SPEC-01.

## Open questions

SPEC-01 §12 (the navigation-quality session).

## Pick-up instruction

Interviewed on 2026-11-01; next is the navigation-quality session, then slice S1.

# Ideas workspace

This is where the owner writes ideas and where agents pick them up. One file per idea,
`YYYY-MM-DD-<slug>.md`, from `TEMPLATE.md`. An idea with only the itch is valid.

## How to write an idea (owner)

Seven short parts, in this order; stop whenever you run out of things to say:

1. **The itch.** What is wrong, missing or slow, one paragraph, in your words. Agents never edit it.
2. **The outcome.** What is true when it is done, stated so someone could check it.
3. **Where it lives.** The repository, service or product surface it belongs to.
4. **Constraints.** Spend, providers, contracts that must not change, deadlines.
5. **Evidence.** Links, prior decisions (ADR ids, answers rows), research, numbers.
6. **Open questions.** What an interview must resolve before anyone builds.
7. **Pick-up instruction.** What an agent should do first: research, prototype, interview, or spec.

Frontmatter: `id` (assigned by `sdlc ideas new <slug>`; until the CLI exists, take the next `ID-n`
from the files here), `title`, `status` (`seed | interviewing | specified | building | shipped |
parked`), `domains` (any of `mission-control`, `knowledge-services`, `aiengineer`, `biotech`,
`agentic-sdlc`), `created`, `owner`, `promoted_to` (program and answers file once interviewed),
`linear` (the `OVE-n` once ticketed).

## How to pick one up (agents)

1. Read this file; list the `status: seed` ideas whose `domains` match your repository.
2. Set `status: interviewing`; run `grill-with-answers` with the idea's `ID-n` as the sitting's
   `Source`; create or choose the program in the owning repository.
3. Never edit the itch paragraph. Fill the other parts only through the interview record.
4. After conversion, write `promoted_to` and `linear` into the idea; set `status: specified`.
5. `sdlc ideas archive <id>` moves a `shipped` or `parked` idea to `archive/`.

The provenance chain from here: idea → interview instrument → answers rows (`Source`) → spec, ADR,
glossary → Linear issue (`## Provenance`) → commits (`OVE-n`). `sdlc trace <id>` prints it.

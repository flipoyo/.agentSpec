# .agentSpec

The generic, project-agnostic half of this owner's agent-facing documents.

Mount this repository at `.agentSpec/` in a consuming project, on its `main`
branch — the same branch for every project, since nothing here is
project-specific. Project-specific references (`AdditionalSpecs.md`,
`audit.md`, a filled-in `AGENT.md`) live in a separate `.localSpec/` mount,
one branch per project — see `DevSpec/DevSpecs.md`'s *Planning* section.

## What is here

- **`TICKETLIFECYCLE.md`** — how a planning ticket under a consuming
  project's own `AgentSpec/` is named and filed: plain name while active, a
  `YYYYMMDD_` stamp and a move to `AgentSpec/archive/` once implemented.
- **`install.cgs`** — this repository's own topology. It mounts
  `flipoyo/DevSpec` at `DevSpec/`, so a project that mounts `.agentSpec`
  with nested discovery enabled gets both in one step.

## What is in `DevSpec/`

The shared philosophy itself, in its own repository so that projects which
mounted it directly keep working:

- **`DevSpecs.md`** — the philosophy; every conforming project follows it.
- **`DOCSTYLE.md`** — the house rule for how any Markdown document in a
  conforming project is written (abstract-first, a mermaid graph, audience
  separation).
- **`AGENT.md`** — a template roster of parallel-agent roles. Copy it to a
  consuming project's own `.localSpec/AGENT.md` and narrow it to that
  project's real scope.

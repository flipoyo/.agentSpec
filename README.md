# .agentSpec

Agnostic development philosophy for agents defined in DevSpecs.md

Using this Specs file accross projects should improve the interoperability of projects

Mount this repository at `.agentSpec/` in a consuming project, on its `main`
branch — the same branch for every project, since nothing here is
project-specific. Project-specific references (`AdditionalSpecs.md`,
`audit.md`, a filled-in `AGENT.md`) live in a separate `.localSpec/` mount,
one branch per project — see `DevSpecs.md`'s *Planning* section.

## Companion files

- **`DevSpecs.md`** — the philosophy itself; every conforming project follows it.
- **`AGENT.md`** — a template roster of parallel-agent roles (Orchestration,
  Dev, CI/CD, Editing, Maths, Scientific editing). Copy it to a consuming
  project's own `.localSpec/AGENT.md` and narrow it to that project's real
  scope.
- **`DOCSTYLE.md`** — the house rule for how any Markdown document in a
  conforming project is written (abstract-first, a mermaid graph, audience
  separation).
- **`TICKETLIFECYCLE.md`** — how a planning ticket under a consuming
  project's own `AgentSpec/` is named and filed: plain name while active, a
  `YYYYMMDD_` stamp and a move to `AgentSpec/archive/` once implemented.


# TODOS

Synthesized from the office-hours design session and CEO review (2026-06-22).
Full context: [docs/design-pm-os-second-brain.md](docs/design-pm-os-second-brain.md).

## P1 — gates everything

- [ ] **T1 — Watch one real PM + run the falsification test (this week, before scaling the build)**
  - Get ONE current PM (not your past self) on a 30-min call. Watch them use AI on a real
    strategy/spec task. Don't demo, don't help. Record the costliest pain moment and what it cost.
  - Falsification test: take one real PM's product context. Produce it two ways — (a) ~30-min
    hand-written plain Claude Project, (b) the structured "guided" version. Run the same 3 real PM
    tasks (strategy memo, spec, prioritization) through both.
  - **Kill criterion:** if a neutral PM can't tell which output used structured context, or
    hand-paste reaches ~80% of the value, the wedge does not exist — stop and rethink before
    building Phases 2-4.
  - **Win payoff:** the before/after comparison becomes the differentiation proof, the shareable
    distribution artifact, and the first-PM hook, all in one.

## P2 — same workstream

- [ ] **T2 — PRD: document the legal-portability foundation as an optional route**
  - Document Option A (5 constraints: own the store, per-object scope field, controlled LLM
    routing, encryption, audit log) as an optional route for the tech team.
  - Mark **own-store + per-object scope field as do-now** (cheap insurance against a multi-tenancy
    rewrite even within the PM product); #3-#5 as the deferrable legal-pivot bundle.

- [ ] **T3 — Instrument context→output traceability from day one**
  - Log which context the brain fed each output, so good vs bad brain evolution is measurable.
  - Also the foundation of the "an update a PM trusts and keeps" success criterion.

## Gate

Phases 2-4 (skill orchestration, second interface, self-evolving brain) do not start until the
T1 falsification test returns a clear "structured wins." Phase 1 build may proceed in parallel
because it produces the test's structured artifact.

## Open questions (carried, not blocking)

- No named current PM yet — T1 forces getting one.
- The PM→lawyer transferable core is still unnamed — revisit once one PM retains.
- Differentiation vs. Claude Projects / ChatGPT memory — T1 is the direct test.

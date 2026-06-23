# PM OS with Second Brain

A product-management operating system built around a **PM Brain** — a plain
markdown second brain that gives AI persistent, structured context about your
product, users, strategy, and decisions. Runs as a Claude Code skill on your
existing Claude Pro/Max subscription.

## The problem

PMs can't use AI for the high-judgment core of their job (strategy, discovery,
prioritization) because AI tools have no memory of their product. Re-explaining
context every session costs more than the output saves. PMBrain is a persistent,
structured context layer that makes AI outputs good enough for real PM work.

## How it works

```
/pm-brain          ← guided 5-batch interview, ~12 min
                   ← or: point at Notion export / Jira CSV / Gong transcript
                   ↓
knowledge/         ← plain markdown folders, local only, never pushed
hypotheses/        ← every claim tagged: documented · verbal · hunch · industry
decisions/
stakeholders/
                   ↓
/discover          ← PM skills that load the brain, run a framework, cite sources
/risk              ← suggest the next command when done
/strategy
...
```

## Status

**Design phase.** Strategy, architecture, and prototypes are complete.
Phase 1 build (the `/pm-brain` guided capture skill) is next.

| Phase | What | Status |
|---|---|---|
| Phase 1 | Guided context builder — `/pm-brain` Claude Code skill | 🔜 building |
| Phase 2 | Skill orchestration — thin hand-wired PM commands | ⏳ gated on T1 |
| Phase 3 | Second interface — web UI when a real user asks for it | ⏳ gated on T1 |
| Phase 4 | Self-evolving brain — built on real usage signal | ⏳ gated on T1 |

**Gate:** Phases 2–4 don't start until a falsification test confirms that
structured context clearly beats hand-pasting into a Claude Project. See `TODOS.md`.

## Repo contents

```
DESIGN.md                        design system (Workbench B tokens, provenance colors)
TODOS.md                         active tasks — T1 gates everything
docs/
  design-pm-os-second-brain.md  full strategy, architecture, and decision log
designs/
  landing-page/                  marketing page prototype
  phase1-guided-capture/         /pm-brain interview prototype
  phase2-skill-layer/            PM skills marketplace prototype
```

## Open the prototypes

```bash
open designs/landing-page/index.html
open designs/phase1-guided-capture/index.html
open designs/phase2-skill-layer/index.html
```

No build step, no server. Each file is self-contained.

## Design system

Dark terminal aesthetic — see `DESIGN.md` for full token reference.
`#070A11` background · `#3DDC84` electric green · Inter UI · JetBrains Mono code.

## Prior art & inspiration

- [PM Brain OS](https://www.productcompass.pm/p/pm-brain-os) — Paweł Huryn
- [PM Skills](https://github.com/phuryn/pm-skills) — 68 skills, 9 plugins, 42 chained workflows
- [Couch to 5K](https://couchto5k.ai) — guided progressive program pattern
- [GBrain](https://github.com/garrytan/gbrain) — self-hostable brain substrate

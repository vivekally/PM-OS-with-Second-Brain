# PM OS — Design Prototypes

Standalone, self-contained HTML prototypes for PM OS. Each `index.html` opens
directly in a browser (no build step, no server). They share the approved
**Workbench** design system: dark slate background, electric-green accent,
Inter for UI and JetBrains Mono for code/data.

The prototypes use a fictional example product, **DataPulse** (a B2B SaaS
activation-analytics tool), throughout.

| Prototype | What it shows |
|-----------|---------------|
| [`landing-page/`](landing-page/index.html) | Marketing page: the second brain, the skill layer, the one loop, and how they compose. |
| [`phase1-guided-capture/`](phase1-guided-capture/index.html) | The `/pm-brain` bootstrap interview — a five-batch guided capture that synthesizes your answers into markdown files with a provenance tag on every claim. Greenfield and migration modes. |
| [`phase2-skill-layer/`](phase2-skill-layer/index.html) | The PM Skills marketplace — commands that chain skills, load the brain (with citations), apply a framework, and suggest the next command. |

## Core concept

The **PM Brain** is plain markdown in a folder (`knowledge/`, `hypotheses/`,
`decisions/`, `stakeholders/`, `ingestion/`, `source/`). Every load-bearing
claim carries a provenance tag — `documented > verbal > hunch > industry` — so
you can see what the brain is leaning on and override it. **Skills** are
workflow modules that run a framework once; the brain is what you know across
all the times you ran it.

## Opening them

```bash
open designs/landing-page/index.html
open designs/phase1-guided-capture/index.html
open designs/phase2-skill-layer/index.html
```

Each `meta.json` records the prototype's design direction, palette, fonts, and
interactive behaviors.

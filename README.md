# AI Interaction Methodology — Public Core

This repository contains the **public core** of the AI Interaction Methodology.

It is the stable public foundation of the system: the canonical artifacts that define its core structure, plus a small supporting layer included only to help explain them. Internal working materials are intentionally excluded.

## Contents

The public core is organized around three canonical artifacts:

* **Methodology** — runtime contract
* **Framework** — reasoning structure
* **Guidelines** — behavioral defaults

Together, these define the methodology’s core public architecture.

## Canonical artifacts

The following files are the authoritative source artifacts in this repository:

* `ai-interaction-methodology/ai-interaction-methodology.md`
* `ai-interaction-framework/framework.md`
* `ai-collaboration-guidelines/ai-collaboration-guidelines.md`

If any supporting material summarizes, interprets, or diagrams the system, these three files remain the source of truth.

## Supporting artifacts

This repository also includes a small supporting layer:

* `supporting/ai-interaction-framework-node-architecture.md`
* `supporting/ai-interaction-methodology-runtime-architecture.md`

These files are explanatory only. They are included to support understanding of the public core, but they are not independent specifications and do not override the canonical artifacts.

## Repository structure

```text
.
├── .github/
│   └── workflows/
│       └── validate.yml
├── ai-collaboration-guidelines/
│   └── ai-collaboration-guidelines.md
├── ai-interaction-framework/
│   └── framework.md
├── ai-interaction-methodology/
│   └── ai-interaction-methodology.md
├── supporting/
│   ├── ai-interaction-framework-node-architecture.md
│   └── ai-interaction-methodology-runtime-architecture.md
├── .gitattributes
├── .gitignore
├── CANONICAL_SOURCE_LOCK.md
├── CLAUDE.md
├── LICENSE
├── OPERATOR_CHECKPOINTS.md
├── README.md
└── what-this-is.md
```

## What is intentionally excluded

This repository is not a full development archive.

It intentionally excludes internal working materials that supported stabilizing the public core.

Those materials are not part of the public canonical surface.

## Recommended reading order

1. `ai-interaction-methodology/ai-interaction-methodology.md`
2. `ai-interaction-framework/framework.md`
3. `ai-collaboration-guidelines/ai-collaboration-guidelines.md`
4. supporting artifacts, if needed

This order preserves the intended separation between runtime contract, reasoning structure, and behavioral defaults.

## Authority and scope

For the public core:

* the three canonical artifacts are the only authoritative source files for canonical semantics
* supporting artifacts may clarify structure, but may not redefine it
* materials outside this repository are not part of the public authority surface unless explicitly incorporated later

Release-lock semantics for the canonical public-core are defined by `CANONICAL_SOURCE_LOCK.md` and the canonical source resolution and compatibility sections of `ai-interaction-methodology/ai-interaction-methodology.md`.

## Purpose

This repository exists to present the methodology’s stable public foundation in a form that is:

* clear
* bounded
* contradiction-free
* easier to read as a system

It is intended to provide a reliable base for understanding, discussion, and future public development.

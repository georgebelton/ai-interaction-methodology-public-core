# Canonical Source Lock

This file defines the pinned public source reference for the canonical public core of the AI Interaction Methodology.

## Canonical Public Repository

`https://github.com/georgebelton/ai-interaction-methodology-public-core`

## Canonical Source Artifacts

The authoritative canonical source artifacts in this repository are:

- `ai-interaction-methodology/ai-interaction-methodology.md`
- `ai-interaction-framework/framework.md`
- `ai-collaboration-guidelines/ai-collaboration-guidelines.md`

## Default Pinned Public Reference

`v1.1.0`

This release tag is the default pinned public compatibility reference for methodology assembly.

## Resolution Rule

A valid public-core methodology assembly must resolve:

- the canonical public repository
- the canonical source artifact path
- the declared pinned reference

Artifacts are considered compatible only if they are resolved from this repository, from the declared canonical file paths, and from the pinned reference declared above.

## Notes

- the declared release tag is the default pinned public compatibility reference
- strict auditability is achieved by resolving the target commit of that declared tag when needed
- the lock file does not record the final release commit SHA for the same release state it defines
- branch names remain invalid as compatibility locks
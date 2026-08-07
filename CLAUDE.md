# AIM Public Core — Working Context

This repo defines the AI Interaction Methodology (AIM): a structured approach to AI
collaboration, published as three canonical artifacts plus two supporting docs. Read
`what-this-is.md` and `README.md` first if you need the full background — the summary
below is only what's needed to work on this repo safely.

## Canonical files (all five, always)

Before proposing or making *any* edit to one of these, read **all five** — not just the
one being changed. They cross-reference each other, and a cut in one can silently break
a claim made in another.

- `ai-interaction-methodology/ai-interaction-methodology.md` — the runtime contract
- `ai-interaction-framework/framework.md` — reasoning structure
- `ai-collaboration-guidelines/ai-collaboration-guidelines.md` — behavioral defaults
- `supporting/ai-interaction-framework-node-architecture.md` — describes how the framework's nodes relate to each other
- `supporting/ai-interaction-methodology-runtime-architecture.md` — describes how the three canonical files relate to each other

Also read `CANONICAL_SOURCE_LOCK.md` before any change that touches file paths, file
names, or the pinned version tag — it must stay in lockstep with reality, not be updated
as an afterthought. It is the source of truth for the current pinned reference; don't
restate that value anywhere else, including here.

## Active task context

Active task context, when present, lives in `NOTES.md` (local-only, gitignored). Check
it before starting work in this repo.

## Working rules

- Confirm which branch is active before making changes; don't switch branches without
  asking. Work happens on a task branch, never directly on `main`.
- Don't commit automatically after edits — stage and describe changes, let the operator
  review and commit.
- **Any whole-section deletion requires a per-claim destination table before staging, at
  the same granularity as a merge.** List each claim in the deleted section and the
  specific line it now lives at. A merge forces this accounting because the content has
  to land somewhere; a deletion lets coverage be asserted without being proved, and that
  asymmetry is where a rule gets lost silently. If a claim's only surviving home is
  several narrower statements rather than one, say so and let the operator decide whether
  the summary is worth keeping — distributed guarantees are harder to keep in lockstep
  under later edits than a single stated one.
- **A deletion's dependency map must be checked in both directions.** What points at the
  content being deleted, *and* what is being kept that points into it. The second
  direction is the one that gets missed, because sequencing cannot fix it: there is no
  "commit this first" that saves a surviving section whose text refers to a deleted one.
  The content itself has to be replaced. Note that resolving a duplication by replacing a
  restatement with a pointer — usually the right call, since it removes a copy that can
  drift — converts a drift risk into a dangling-reference risk, and the deletion map is
  where that debt comes due.
- **A dangling-reference repair is only durable if its new location survives the rest of
  the plan, not just the current commit.** Inlining content into a surviving section
  fixes the break at hand; check that section against the full remaining deletion
  schedule before treating the repair as done. This is the temporal extension of the
  both-directions rule above, which asks what a deletion points at and what points at it
  — both evaluated against a single commit. It does not ask whether the place the content
  just landed is itself scheduled for removal, and a repair made toward the deletion
  frontier buys exactly one commit.
- After any term-driven cross-reference search, do one full non-term-driven read of the
  affected file before treating the map as complete. Every time this has been done it
  found something the search missed. Keyword search fails in at least four distinct ways,
  and each was observed producing a real undercount:
    - **paraphrase** — a renamed label carrying the same meaning (`Authority + Execution
      Controls` for an execution-state reference)
    - **concept vs word** — the idea stated without its keyword (searching "downgrade"
      found 3 of 28; searching the concept found the rest)
    - **proximity miscategorization** — content bucketed by the section containing it
      rather than by what it says, so it does not read as the thing being searched for
    - **negative phrasing** — the same obligation stated inverted, sharing no keywords
      with the positive form (`must not silently continue` for a disclosure requirement;
      searching only the positive form found 15 of 32)
  A count that stops where the first search ended is almost certainly short. State the
  search that was run, not the conclusion drawn from it.
- For byte-level checks (line endings, encoding, whitespace), use methods immune to
  shell-quoting loss: `git cat-file -p` for raw blob content (`git show` can apply
  filters), `tr -dc '\r' | wc -c`, or a direct read in python. Do **not** use `grep` with
  ANSI-C quoted patterns — `$'\r'` can lose its escaping through nested quoting and
  degrade to a pattern matching every line. The result then looks like a plausible count
  rather than an error, so the failure is silent.
- If a section's purpose is unclear, ask rather than guess. Getting this repo's own
  epistemics wrong while editing a methodology about reasoning discipline is the kind of
  irony worth avoiding.

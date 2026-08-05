# Operator Checkpoints

**This is not a canonical artifact.** It is not one of the three canonical source
artifacts declared in `CANONICAL_SOURCE_LOCK.md`, it defines no rules, and it overrides
nothing. Every question here is derived from a canonical rule and cites where that rule
lives.

## Why this exists

Part of the methodology was written as prose asking the model to privately track state
across turns — execution states, halt states, re-entry conditions, loop counters. A model
cannot reliably hold that state, so stating it as a rule produced the appearance of
control rather than control itself. The underlying checks are worth keeping. They just
have to be performed by a person at a checkpoint, where the answer can actually be
observed.

**None of these questions define anything.** If an entry below starts explaining a rule
in its own words instead of pointing at the methodology's statement of it, it has become
a second source of truth and should be corrected back to a pointer.

## When to run these

At any point where you would otherwise be relying on the model's own account of whether
it is authorized to proceed:

- before substantive work begins on an artifact-bound task
- when the model reports being blocked, or resumes after having been blocked
- when the same question has been revisited without resolving
- before accepting output as complete

## The checks

### 1. Entry conditions

**Were the required entry checks actually performed, or only claimed?**

Ask for the evidence, not the assertion: which artifacts were read, at what version, and
when. "I have the context" is not an answer.

*Canonical rules:* Bootstrap Entry Rule · Active Artifact Set Resolution · Grounding
Preflight Requirement.

---

### 2. Stop conditions

**Is there a stop condition in effect right now?**

If yes: what specifically is blocked, and what would unblock it? A stop condition that
cannot name what it is waiting for is not being enforced.

Note that requesting clarification, override, or scope narrowing is permitted while
stopped — those are the only ways a stop ends.

*Canonical rules:* Halt-State Classification Rule · Blocked Execution State (see Allowed
Actions in Blocked State for what remains permitted).

---

### 3. Resumption basis

**If work resumed after a stop, what specifically authorized it — and how far?**

The answer must name something that actually changed. Conversational momentum, elapsed
turns, and inferred intent are not authorization. Resumed scope should not exceed the
scope of whatever authorized it.

*Canonical rules:* Halt Re-entry Rule.

---

### 4. Repetition without progress

**Has this been attempted before without new information?**

If the same unresolved question is being worked a second time and nothing new has come
in, stop and ask rather than attempt it again. Reformulating the question is not new
information.

*Canonical rules:* Uncertainty-Loop Budget Rule.

---

### 5. Narration in place of action

**Is the model describing work instead of doing it, or stopping?**

Readiness statements, restated intentions, and preparatory framing are not progress. Once
preconditions are met there are two valid outcomes: do the work, or stop and say why.

*Canonical rule:* see the methodology's statement of this invariant — do not restate it
here.

---

## Recording the answers

There is no required format. What matters is that the answers are observable by someone
other than the model, and that a "yes" is backed by something checkable rather than
asserted.

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
- **`gh` is authenticated here, so the delegation boundary is a written rule rather than a habit.**
  The agent **may open PRs and may read anything** — repository settings, rulesets, branch
  protection, merge methods, releases, workflow runs. **These come to the operator: merging a PR;
  creating or editing a GitHub Release; anything touching a published ref** (tags, `main`, branch
  deletions); **any repository settings change — and committing**, which is not new: it is already
  reserved by *"stage and describe changes, let the operator review and commit."* The rest are what
  `gh` newly made reachable; **this list is not the whole boundary.** The line is reversibility —
  *opening a PR is reversible and reviewable; merging is not.* It is written down because the tool
  removed an enforcement that had been structural: before `gh`, the merge-method choice, the Latest
  toggle and the linear-history setting each reached a person **because the agent could not reach
  them**, and each was a point where being forced to stop was load-bearing. `gh pr merge --squash`
  is now as easy to type as `--rebase`, and the consequence — orphaning a published tag — is **one
  flag from silent**. Settings are the sharpest case: the agent can now *create* environment
  changes that leave no trace in the repository rather than only observe them. Stopping at every
  irreversible step is **part of the safeguard, not a substitute for the rule**, which exists so
  the boundary does not depend on being remembered.
  **Pushing a task branch is inside the boundary, and so is force-pushing one** — but a force-push
  to a branch with an open PR rewrites the object the operator is reviewing against, and nothing on
  the server notices: `non_fast_forward` covers only the default branch, and no approval is
  required. So it carries the history-rewrite record below, and **the new head SHA must be stated in
  conversation**, so the merge is against a known object rather than the latest one.
  **Where this meets *attempt the refusable operation first*:** the cheap test for whether a policy
  will refuse something is a throwaway attempt, but **the attempt is sometimes the reserved
  operation itself** — a merge method can only be shown unavailable by trying to merge. Then the
  probe comes to the operator, and where the rule already settles the question, decide on the rule
  rather than wait. **An unrunnable probe is not a blocker.**
- **A history-rewriting operation must be recorded in `NOTES.md` when it happens**, in the
  same per-commit pattern as any other commit, naming **both** hashes — the new one and the
  one it discarded — and what the rewrite changed and why. Amend, rebase, and reset are the
  cases. This is a recording requirement, not a prohibition: amending before push is often
  correct, as when a commit's own text violates the rule it establishes. But **disclosure in
  conversation is not the record.** Prose scrolls away, and the discarded hash in particular
  tends to go unnamed because it no longer appears in `git log` — so a rewrite that exists
  only in chat leaves the durable record with a hole exactly where history diverged from what
  was reported. The hole is worst where it is most load-bearing: an undescribed object cannot
  be reasoned about, and should never be the subject of a request to delete it.
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
  where that debt comes due. **Sweep five reference classes, not one: section names,
  defined terms, references to the *category* a section established, positional pointers,
  and indices.** The third is the one no term search can reach, because what is referenced is
  the taxonomy rather than any member of it — a surviving "not a substitute bootstrap
  state" survives every search for the states themselves. The fourth needs a pattern wider
  than it looks: `defined separately below` defeats a pattern written for `defined below`.
  Terms also appear as bare adjectives, so search the one-word form as well as the phrase.
  The fifth escapes on **the role it plays in the sentence, not its token shape**: a span
  cited as a *measurement* of a section reads as data rather than as a pointer into it, and
  two independent sweeps missed one for that reason. **An index is a reference; the content
  is the locator.** Line numbers, ordinals and counts are all indices, each invalidated by a
  different operation — **insertion invalidates line numbers and ordinals, compression
  invalidates counts.** A bare `:NNN` cannot even be swept, since a line number in one file
  and in another are syntactically identical, so **a citation must name its file** and a rule
  is cited by its opening words, never its position. A claim about what was *said* names its
  channel the same way: *"not in my context"* is not *"never said."*
  **A clean sweep is not a clean result** — do the full read afterward; every time these
  classes have been added, it was because the earlier sweeps returned clean and were wrong.
- **A dangling-reference repair is only durable if its new location survives the rest of
  the plan, not just the current commit.** Inlining content into a surviving section
  fixes the break at hand; check that section against the full remaining deletion
  schedule before treating the repair as done. This is the temporal extension of the
  both-directions rule above, which asks what a deletion points at and what points at it
  — both evaluated against a single commit. It does not ask whether the place the content
  just landed is itself scheduled for removal, and a repair made toward the deletion
  frontier buys exactly one commit. **The same applies to per-claim destination-table
  entries: a claim's cited surviving home must itself be checked against the remaining
  deletion schedule, not merely confirmed to exist today.** Citing coverage and placing
  content are the same assertion — *this claim now lives at X* — so if X is scheduled for
  deletion the table is wrong in precisely the way this rule exists to prevent. The
  asymmetry that makes this easy to miss: placing content feels like an edit and invites
  the durability check, while citing a location feels like an observation and does not.
- **Correct live statements; annotate dated ones.** A statement making a claim about *now*
  misdirects the next piece of work if it is wrong, so fix it in place. A dated record *was*
  true when written, and editing it rewrites the ledger — destroying the evidence of how a
  figure moved, which is the only thing that makes a corrected figure auditable rather than
  merely asserted. The test is not "is this current" but **"is this statement making a claim
  about now."**
- **A numeric target on a document is a proxy.** When a pass moves the metric without
  improving the artifact — a rewrap, a separator, a reflow — the target has become the goal.
  **Report the number and stop rather than finding another line.** The reverse direction
  needs stating too: when a genuine improvement happens to move the number, say which it was,
  because a cut made to hit a threshold and a cut made for readability are indistinguishable
  from outside.
- After any term-driven cross-reference search, do one full non-term-driven read of the
  affected file before treating the map as complete. Every time this has been done it
  found something the search missed. Keyword search fails in at least four distinct ways,
  and each was observed producing a real undercount:
    - **paraphrase** — a renamed label carrying the same meaning (`Authority + Execution
      Controls` for an execution-state reference)
    - **concept vs word** — the idea stated without its keyword (searching "downgrade"
      found 3 of 28; searching the concept found the rest)
    - **proximity miscategorization** — content bucketed by the section containing it
      rather than by what it says, so it does not read as the thing being searched for.
      The same error occurs one level down: content bucketed by **its own heading** rather
      than by what it says. A `Purpose` heading held eleven `must` statements; five
      subsections named for control states turned out to be permissions and
      non-establishment gates. Classify by reading the body, never by the heading — and
      treat a scope estimate built from headings as unmeasured, whichever direction it
      later moves
    - **negative phrasing** — the same obligation stated inverted, sharing no keywords
      with the positive form (`must not silently continue` for a disclosure requirement;
      searching only the positive form found 15 of 32)
- **State the search that was run, not the conclusion drawn from it**, and **a verification
  predicate must be at least as wide as the defect it has just found.** A count that stops
  where the first search ended is almost certainly short. A sweep written to catch stale
  citations required a filename prefix while the site it had just repaired carried a bare
  one — so the check passed, and could not have caught its own class. The failure is
  symmetric: too narrow under-reports, too broad over-reports, and **an over-flagging check
  erodes trust in the check**, which is how a real hit later gets waved through as one more
  false positive. **Classify sweep hits, do not count them** — that applies to your own
  guards, not only to the text under review.
- For byte-level checks (line endings, encoding, whitespace), use methods immune to
  shell-quoting loss: `git cat-file -p` for raw blob content (`git show` can apply
  filters), `tr -dc '\r' | wc -c`, or a direct read in python. Do **not** use `grep` with
  ANSI-C quoted patterns — `$'\r'` can lose its escaping through nested quoting and
  degrade to a pattern matching every line. The result then looks like a plausible count
  rather than an error, so the failure is silent. Two more members of the same family, both
  where the medium mangles the text before the check sees it:
    - **The file-editing tool writes CRLF on this platform.** Observed converting two whole
      files — every line, not just the edited region — where files written by python with
      `newline='\n'` had none. `.gitattributes` pins `eol=lf`, so the *commit* is clean
      either way and looks clean; but that file's stated intent is a working copy
      byte-identical to what git stores, because the risk is raw working-tree bytes being
      packaged into an artifact. Prefer python writes with `newline='\n'` for tracked files,
      or byte-check after every edit.
    - **A newline defeats a grep pattern.** `seven.*against fourteen` returned zero because
      the text wrapped between `seven` and `paths`. Flatten newlines before grepping
      multi-line prose, or match a fragment short enough that it cannot wrap. This is the
      third instance of a pattern narrower than the text it checks.
- **A measure can be accurate and still answer a different question than the one it is used for.**
  This case shares the outcome of the shell-quoting family in *"For byte-level checks"* but not
  its mechanism: there the medium altered the text before the check read it, whereas here **a name
  did not describe the contents**. A GitHub Release's `created_at` is the *tag object's* date, not
  when the Release was published — `published_at` is that, and sat in the same response unread.
  Reading the label as the fact it appears to state produced a reported anomaly that did not
  exist, and then an explanation for it, which no evidence could have contradicted because there
  was nothing there. `git status` reporting "ahead by N" against a stale tracking ref is the same
  shape, and so is a diffstat: **an edit framed as an insertion can carry a deletion, and `N
  insertions / 0 deletions` against `HEAD` cannot show it** when the whole block is new, so an
  intra-session cut stays invisible inside a number that is perfectly correct. **Check what a
  measure measures before building on it, read the sibling field, and diff against the last
  reviewed state rather than only against `HEAD`** — record the reviewed blob (`git rev-parse
  :<file>`) so the next check is `git diff <recorded-sha> :<file>`, computed rather than asserted.
- **A verification whose success condition is "no matches" must not be chained on its exit
  status.** `grep`/`grep -c` exit non-zero on zero matches, so the command confirming *"no
  occurrences remain"* reports shell-level failure exactly when the news is good. Chained
  with `&&`, or under `set -e`, that aborts the script partway — and it aborts the run that
  was verifying the correct result, so what surfaces is a broken check rather than a passing
  one. Assert the count explicitly (capture it and compare), or append `|| true`. Same
  silent-failure shape as the `$'\r'` case above: the outcome looks like a legitimate
  negative rather than a malfunction, which is why neither is caught by reading the output.
- **Never cite the operator's internal failure records in this repo.** Work here may be
  informed by private incident and root-cause documentation held outside the repo. Nothing
  committed to public-core — commit messages, file content, comments — may name those
  documents, quote them, describe their structure, or reference their existence. Cite the
  *class of failure* instead: "addresses a documented evidence-handling failure" is fine;
  identifying the record it came from is not. The leak is structural rather than textual —
  naming a document discloses that it exists, what it covers, and how the private record is
  organised, none of which a public repo should reveal. This applies to paraphrase, and to
  counts and enumerations, as much as to titles — stating how many records exist, or of what
  kinds, is the same disclosure by a different route.
- **Before an operation a server policy could refuse, check the policy — not just the object
  graph — and attempt the refusable operation first.** Ancestry, ahead/behind, merge-base and
  `git ls-remote` all read the commit graph; push permission is not a property of the commit
  graph, and `ls-remote` reads refs, not rules. A fast-forward can be verified as available,
  repeatedly and against the server, and still be forbidden. Where a sequence contains one
  step that might be refused, do that step first: a `main` push rejected by branch protection
  after a tag had already been pushed left a published release the default branch did not
  contain, *and* foreclosed fixing anything in that release without re-signing the tag. One
  ordering choice cost both the consistency and the remedy. The cheap form of this is a
  throwaway attempt — verifying that tag signing worked on a scratch tag, before deleting a
  published one, is what kept a delete-then-fail-to-recreate out of the sequence.
  **Three further checks answer a narrower question than their names suggest.**
  `--is-ancestor` is **permanently wrong wherever rebase or squash is the merge method**,
  since both destroy ancestry by construction, so it answers no forever for a fully merged
  branch; use `git cherry`, which takes any commit-ish and so still works after the branch
  ref is gone. **A branch-protection endpoint can return 404 while the branch is protected**,
  because the policy lives in a ruleset at a different endpoint — and two endpoints describing
  one ruleset return different field sets. **A required status check pins a job's
  display-name string**: appending jobs is safe, renaming or splitting one leaves PRs pending
  rather than failing, and the repair is a settings change rather than a file edit.
- **Release tags must be signed, and every release tag gets a GitHub Release.** `git tag -a`
  does not sign; `git tag -s` does, and `tag.gpgSign=true` makes it automatic. Verify with
  `git cat-file -p <tag>` before pushing, and re-verify after, because the signature has to
  survive the round trip. Release notes live in GitHub's database rather than the tag object,
  so a signed tag with no Release is still an incomplete release. Signing matters here
  specifically: `CANONICAL_SOURCE_LOCK.md` makes the release tag the pinned reference for all
  canonical resolution and the bootstrap rules turn on exact artifact identity, so an unsigned
  tag is a name anyone with push access could have created.
  **The general hazard, which is why both of these are written down at all: automating a manual
  sequence captures the steps and drops the tacit practices attached to them.** Signing and
  publishing a Release were both habits in a person's hands, so writing down the sequence
  captured everything except the parts that were never written down. Two independent gaps, one
  cause, and neither was noticed until someone compared a new release against an old one.
- If a section's purpose is unclear, ask rather than guess. Getting this repo's own
  epistemics wrong while editing a methodology about reasoning discipline is the kind of
  irony worth avoiding.

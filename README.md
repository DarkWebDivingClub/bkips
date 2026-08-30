# BKIPs — Bitcoin Knots Improvement Proposals

Specifications for changes to Bitcoin Knots, written where none exist.

Bitcoin has BIPs. The Knots fork — in particular the BLAKE2b
proof-of-work change — has no equivalent: the authority is a pull
request and the C++ that implements it. Anyone building against it has
to read the source and infer the rest.

These documents write that down. They are descriptive, not normative:
**where a BKIP and Knots disagree, Knots is correct and the BKIP is
stale.** Each one names the source it was written from, so it can be
rechecked when that source moves.

## Index

| # | Title | Status |
|---|-------|--------|
| [0001](bkip-0001.md) | The v2 block header | Draft |

## Numbering and status

Numbers are assigned in order and never reused. A document keeps its
number if superseded; the superseding one says so.

| Status | Meaning |
|---|---|
| Draft | Being written; may be wrong or incomplete |
| Verified | Checked against the source and its test vectors, and against at least one independent implementation |
| Stale | The change it describes has moved on |

**Verified means checked, not reviewed.** A document reaches it only
once something has been implemented from it and agrees — a
specification validated only against the notes it was written from
propagates its own errors.

## Conventions

- One change per document.
- Say what the source of truth is, by file and branch, at the top.
- Mark unknowns as open questions rather than guessing. Design intent
  is not recoverable from code, and inventing plausible reasons is how
  a specification becomes actively misleading.
- No project-specific content. These describe Knots, not what anyone
  builds on it.

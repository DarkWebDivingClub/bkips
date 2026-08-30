# BKIPs — notes on Bitcoin Knots consensus changes

## Read this first

**This is a temporary place to write things down, not a process.**

It is not affiliated with, endorsed by, or coordinated with Bitcoin
Knots or its maintainers. It does not assign anything, does not confer
status on anything, and has no authority over anything. The numbering
mirrors BIP style because that shape is familiar, not because a series
is being claimed. Nobody needs anyone's permission to write down how
something works, and that is all this is.

These documents exist because implementing against the Knots consensus
changes required reading C++ and inferring the rest, and writing that
down was cheaper than doing it twice. They are published so the next
person does not repeat the reading.

**They are descriptive, and they are provisional.** Where a document
and Knots disagree, **Knots is correct and the document is wrong**. If
Knots publishes a specification of its own, or a BIP appears, that
supersedes everything here and these should be marked Stale and left
alone. That would be the good outcome: this exists only because nothing
else does.

Corrections are welcome from anyone, particularly from people who wrote
the code being described.

## Terminology

**Bitcoin Knots (BTK)** is the consensus branch created by the BLAKE2b
proof-of-work change, as distinct from **BTC**. "Knots" alone refers to
the software; **BTK** refers to the chain and its consensus rules, and
is used wherever the branch is the thing that matters.

## Index

| # | Title | Status |
|---|-------|--------|
| [0001](bkip-0001.md) | The BTK v2 block header | Draft |

## Numbering and status

Numbers are assigned in order and never reused. A document keeps its
number if superseded; the superseding one says so.

| Status | Meaning |
|---|---|
| Draft | Being written; may be wrong or incomplete |
| Verified | Checked against the source and its test vectors, and against at least one independent implementation |
| Stale | Superseded, or the change it describes has moved on |

**Verified means checked, not reviewed.** A document reaches it only
once something has been implemented from it and agrees — a
specification validated only against the notes it was written from
propagates its own errors.

## Conventions

- One change per document.
- Say what the source of truth is, by file and branch, at the top.
- Mark unknowns as open questions rather than guessing. Design intent
  is not recoverable from code, and inventing plausible reasons is how
  a description becomes actively misleading.
- No project-specific content. These describe BTK, not what anyone
  builds on it.

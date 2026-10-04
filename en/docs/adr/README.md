<!-- mirror-of: docs/adr/README.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [docs/adr/README.md](../../../docs/adr/README.md). The Chinese version is authoritative.

# Architecture Decision Records (ADRs)

An ADR records a **major decision** and the reasoning at the time, so later readers (including future us) know why it was done this way.

## When to write one

Only when **all three** hold:

1. **Hard to reverse:** changing our minds later would be costly (e.g. switching databases, changing Time Coin rules).
2. **Surprising without context:** a future reader would ask "why did they do it this way?"
3. **A real trade-off:** there were viable alternatives and we picked this one for specific reasons.

Ordinary decisions just go in [LOG.md](../../LOG.md).

## Format

Filename: `NNNN-short-english-title.md`, e.g. `0001-postgresql-as-database.md`. Numbers increase sequentially.

```markdown
# NNNN. Title

- **Date:** YYYY-MM-DD
- **Status:** Proposed / Accepted / Superseded by NNNN

## Context

The problem and constraints.

## Decision

What we decided.

## Options considered

- Option A: pros / cons
- Option B: pros / cons

## Consequences

What follows from the decision, good and bad.
```

(Teammates write ADRs in Chinese, following the Chinese template.) After writing an ADR, add a LOG.md entry linking it.

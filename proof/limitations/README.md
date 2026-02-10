# Known Limitations

This directory documents **architectural boundaries** and **scope limitations** of the current proof.

---

## Purpose

These are not bugs or failures.
These are **documented constraints** of what this demo proves and does not prove.

> **Honest engineering > marketing spin.**

---

## Current Limitations

### [SEMANTIC_VARIANCE.md](SEMANTIC_VARIANCE.md)

**Status:** Known architectural limitation
**Impact:** Pattern-based detection, not effect-based convergence

**What it means:**
- Different phrasings of similar intent do not converge to same decision
- Example: `"delete files"` → STOP, but `"clean up directories"` → ALLOW
- Semantic variance handling requires action abstraction layer (out of scope)

**What it does NOT invalidate:**
- ✅ Boundary effectiveness (execution stops when triggered)
- ✅ Audit trail (decisions are logged)
- ✅ Non-execution guarantee (e.g., payment never called)

---

## Why We Document Limitations

1. **Credibility:** Acknowledging constraints builds trust
2. **Scope clarity:** Prevents misinterpretation of claims
3. **Design transparency:** Shows what's proven vs what's future work
4. **Attack surface management:** Pre-empts criticism by addressing it proactively

---

## What This Does NOT Mean

❌ "The demo is broken"
❌ "The proof is invalid"
❌ "The boundary doesn't work"

✅ **"The boundary works when triggered. Trigger coverage is pattern-based, not effect-based."**

---

## How to Read These Documents

Each limitation document contains:
- **Observation:** What behavior was observed
- **Interpretation:** What it means architecturally
- **Scope:** What's affected vs what's not affected
- **Next Steps:** What would be required to address it (if out of scope)

---

## Communication Guidelines

### Internal
> "We've documented the boundaries of what this proof covers. Semantic variance is a known limitation that requires action abstraction."

### External
> "This demo proves the boundary stops execution when triggered. Semantic paraphrase handling is intentionally out of scope for this structural proof."

### If Challenged
> "Correct. That's a documented limitation. The boundary mechanism is proven. Detector sophistication is the next layer."

---

## Related Documentation

- [../../README.md](../../README.md) — Main project documentation
- [../../ANTICIPATED_QUESTIONS.md](../../ANTICIPATED_QUESTIONS.md) — Q&A addressing common critiques
- [../../HARDCODING_DEFENSE_COMPLETE.md](../../HARDCODING_DEFENSE_COMPLETE.md) — Hardcoding rationale

---

## Summary

**Purpose:** Transparent documentation of scope boundaries
**Status:** Proactively disclosed, not hidden
**Impact:** Strengthens credibility through honesty

> **"We document what we prove and what we don't.
> This is how honest engineering works."**

---

**Last Updated:** 2026-02-11

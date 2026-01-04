# Canonical State Taxonomy

## Principle

Participants may attest **only what they know with certainty**.

---

## Allowed States

### ACCEPTED
Transaction request accepted and LTID recognized.

### PROCESSED
Participant completed its internal responsibility.

### REJECTED
Participant definitively failed the transaction.

### UNKNOWN
Participant cannot assert a definitive state.

Includes:
- timeout
- downstream opacity
- system uncertainty
- operational gaps

---

## Prohibited States

Participants MUST NOT attest:
- progress percentages
- speculative outcomes
- optimistic assumptions
- internal workflow steps

Silence is valid and maps to UNKNOWN.

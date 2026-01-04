# Logical Transaction Identifier (LTID)

## Purpose

LTID represents **one real-world payment**
across multiple independent systems and ledgers.

It is the minimum shared anchor required
to correlate transaction states safely.

---

## Mandatory Properties

LTID MUST:
- be globally unique
- be immutable
- be created exactly once
- be propagated across participants
- be independent of internal references

LTID MUST NOT encode:
- customer identity
- account information
- amount or currency
- participant identity
- routing data

---

## Creation

- Created at transaction initiation
- Created by sender bank or initiating switch
- Exactly one LTID per logical transaction

---

## Mapping

Each participant maintains a **private mapping**:

internal_reference → LTID


This mapping is never shared.

---

## Non-Goals

LTID is NOT:
- proof of settlement
- proof of success
- reconciliation guarantee

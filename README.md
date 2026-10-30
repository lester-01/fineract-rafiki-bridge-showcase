# Fineract ↔ Rafiki Bridge

**[Open the case study → fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me)**

A TypeScript bridge that lets **Apache Fineract** savings banks act as Account Servicing Entities behind **Rafiki** (Interledger / Open Payments). Fineract stays the ledger of record. Rafiki moves the payment.

## Why it matters

Core banking and Open Payments speak different languages. This bridge is the ASE glue:

- **Hold before liquidity** — `availableBalance` → hold → fund outgoing payment (never debit on `accountBalance` alone)
- **Quote-then-pay** — Admin GraphQL initiation without a mid-quote pause
- **Signed webhooks** — `Rafiki-Signature` over timestamp + RFC 8785 canonical JSON, with idempotent handlers
- **LedgerAdapter** — flows depend on an interface; Fineract savings is implementation #1

## Proof

- **Three banks · two Rafiki nodes** — intra-bank, same-Rafiki cross-bank, and cross-Rafiki transfers
- **Money journey** — follow one $15 cross-instance payment through the send UI, both Rafiki Admins, and both Mifos ledgers (screenshots on the site)
- **Engineering gates** — CI (lint · typecheck · Vitest), **151** unit tests including idempotency, Bruno live API collections, containerized demo network, `business-test` matrix

Sandbox demo is available **on demand** (the playground is resource-heavy). The case study leads with recorded proof.

## Links

| | |
|---|---|
| **Case study** | [fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me) |
| **All projects** | [projects.benlester.me](https://projects.benlester.me) |
| **Resume** | [benlester.me](https://benlester.me) |

Built by **Ben Lester** — Software & Systems Engineer.

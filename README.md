# Fineract ↔ Rafiki Bridge

**[Open the case study → fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me)**

The bridge between core banking and Open Payments. This case study shows a money-safe integration layer for an Account Servicing Entity: the bank keeps its own ledger while customers send and receive through Open Payments and Interledger.

## What it demonstrates

- **ASE ↔ payment-node bridge** — holds before liquidity, signed webhooks, idempotent audit
- **Swappable ledger adapter** — Apache Fineract savings is the demo ASE; the same money rules apply when another core system is wired in
- **Domestic and cross-border class of problem** — peered Rafiki instances and Open Payments paths; this demo runs single-currency USD across three banks and two Rafiki nodes
- **Engineering gates** — CI, 151 unit tests, Bruno live collections, containerized three-bank proof

## Live demo

The sandbox is available **on request** (it is resource-heavy). Prefer a walkthrough over a static page? Email [contact@benlester.me](mailto:contact@benlester.me?subject=Live%20demo%20%E2%80%94%20Fineract%E2%80%93Rafiki%20bridge).

## Links

| | |
|---|---|
| **Case study** | [fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me) |
| **All projects** | [projects.benlester.me](https://projects.benlester.me) |
| **Resume** | [benlester.me](https://benlester.me) |

Built by **Ben Lester** — Software & Systems Engineer.

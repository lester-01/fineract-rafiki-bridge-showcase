# Fineract ↔ Rafiki Bridge

**[Open the case study → fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me)**

Integration layer that lets a bank-style ledger (Apache Fineract) send and receive payments over Open Payments and Interledger via Rafiki, while the ledger stays the source of truth. Runs as a three-bank sandbox with virtual funds.

## What it demonstrates

- **ASE ↔ payment-node bridge** — holds before liquidity, signed webhooks, idempotent audit
- **Swappable ledger adapter** — Apache Fineract savings is the demo ASE; the same money rules can be rebuilt in TypeScript, Python, Go, JavaScript, or Java
- **Bank-initiated sandbox** — wallet addresses for active accounts; pay by address, not account number
- **Beyond the demo** — client/merchant authorization, checkout, and recurring Open Payments flows are not wired here
- **Engineering gates** — CI, unit tests, Bruno live collections, multi-node three-bank proof

## Live demo

The sandbox is available **on request** (it is resource-heavy). Prefer a recording? Start with [chapter 09 (~7 min) on the case study](https://fineract-rafiki.benlester.me/#video-09), or email [contact@benlester.me](mailto:contact@benlester.me?subject=Live%20demo%20%E2%80%94%20Fineract%E2%80%93Rafiki%20bridge).

## Links

| | |
|---|---|
| **Case study** | [fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me) |
| **All projects** | [projects.benlester.me](https://projects.benlester.me) |
| **CV** | [benlester.me](https://benlester.me) |

Independent project. Not affiliated with or endorsed by Apache Fineract, Mifos, or the Interledger Foundation.

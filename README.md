# Fineract ↔ Rafiki Bridge

**[Open the case study → fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me)**

I built an integration layer that lets a bank-style ledger (Apache Fineract) send and receive payments over Open Payments and Interledger, using Rafiki, while the ledger stays the source of truth. It runs as a three-bank sandbox with virtual funds.

## What it demonstrates

- **ASE ↔ payment-node bridge** — holds before liquidity, signed webhooks, idempotent audit
- **Swappable ledger adapter** — Apache Fineract savings is the demo ASE; the same money rules can be rebuilt in TypeScript, Python, Go, JavaScript, or Java
- **Why bridge at all** — remittance-style corridors, domestic interoperability, and ledger authority; Mojaloop-class clearing is adjacent work (not used in this stack)
- **Engineering gates** — CI, 152 unit tests, Bruno live collections, containerized three-bank proof
- **Honest limits** — sandbox with virtual funds; peer settlement and production ASE requirements called out on the case study

## Live demo

The sandbox is available **on request** (it is resource-heavy). Prefer a walkthrough over a static page? Start with [chapter 09 on the case study](https://fineract-rafiki.benlester.me/#video-09), or email [contact@benlester.me](mailto:contact@benlester.me?subject=Live%20demo%20%E2%80%94%20Fineract%E2%80%93Rafiki%20bridge).

## Links

| | |
|---|---|
| **Case study** | [fineract-rafiki.benlester.me](https://fineract-rafiki.benlester.me) |
| **All projects** | [projects.benlester.me](https://projects.benlester.me) |
| **CV** | [benlester.me](https://benlester.me) |

Built by **Ben Lester** — Freelance Software & Systems Engineer.

Independent project. Not affiliated with or endorsed by Apache Fineract, Mifos, or the Interledger Foundation.

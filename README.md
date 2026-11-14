# Furkan Derse

One surface. Five business days. **$1,500.** The deliverable is a private repo and a walkthrough, not a PDF and not an audit stamp.

Site: [dersefurkan.github.io](https://dersefurkan.github.io) · dersefurkan32@gmail.com · Telegram [@FURY_Fn](https://t.me/FURY_Fn)

A written scope comes before any test. I do not test systems I am not hired to review.

## Surfaces

| Surface | What you send | Price |
| --- | --- | --- |
| Contract or zkVM seam | One contract family, one diff under 800 lines, or one guest plus its verifier | $1,500 |
| Web app | One staging app, one role, the flows named in the scope | $1,500 |
| AI agent | One staging chat or tool endpoint, the tools and data named in the scope | $1,500 |

A second surface is a second pack, after the first repo is delivered. Terms: [SERVICES.md](SERVICES.md).

## What the five days cover

- **Contracts and zk.** Invariant or fork tests on the identity that moves the money. Guest program plus the verifier that checks it.
- **Web.** The flows in scope, checked against the OWASP Top 10 (2021) categories that those flows actually touch. Evidence is a request and the state after it, not a scanner score. Map: [WEB.md](WEB.md).
- **AI agent.** Whether a tool call, a document, or another tenant changes something the product did not allow. The model’s sentence is not the proof. Map: [AI.md](AI.md).

Each pack includes a property table, a failing test or a request log when a named property breaks, one walkthrough, and a 14-day fix re-run.

## Public samples

| Repo | What it shows |
| --- | --- |
| [split-ledger-vault-demo](https://github.com/dersefurkan/split-ledger-vault-demo) | Money-moving identity. Split ledgers and a missing queue cursor. Directed tests, then conservation and per-request invariants on the patched vaults. |
| [pool-invariant-suite-demo](https://github.com/dersefurkan/pool-invariant-suite-demo) | First-depositor inflation and performance-fee creep. Handler invariants, cross-checks, storage-layout drift. 32 tests. |
| [risc0-onchain-verify-demo](https://github.com/dersefurkan/risc0-onchain-verify-demo) | Rust guest to Groth16 receipt to Solidity verifier. Negative tests for a tampered journal, a wrong image ID, and a bad selector. |
| [zkvm-guest-bug-notes](https://github.com/dersefurkan/zkvm-guest-bug-notes) | Guest-program and on-chain binding classes. Public references only. |

The AI lab note in [AI.md](AI.md) is the same kind of sample. Teaching results. Not a finding against a live product.

## The limit

This is a security review of the named surface. A green result means the tested properties held under the tested conditions. It is not a claim that the product is safe.

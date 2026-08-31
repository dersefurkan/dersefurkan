# Furkan Derse

Independent security reviewer for DeFi protocols and zkVM integrations.

The deliverable is a private Foundry repo with green `forge test` output — not a PDF.

## Work

- **Invariant suites** — stateful fuzzing around the identity that actually moves money: receipt ids, epoch indices, match ids, withdrawal cursors, forwarder senders.
- **Mainnet-fork tests** — against a live deployment or a pinned commit, authorized scope only.
- **Upgrade / diff review** — a focused pass over what changed after a proxy upgrade or a patch.
- **zkVM / coprocessor boundary** — guest program plus on-chain verifier binding: image ID pinning, journal commitment, replay resistance.

This is a time-boxed **security review**, not a security audit and not a guarantee. Terms: [SERVICES.md](SERVICES.md).

## Public samples

| Repo | What it shows |
| --- | --- |
| [split-ledger-vault-demo](https://github.com/dersefurkan32-dotcom/split-ledger-vault-demo) | Split-ledger identity: one deposit, two independent claims. Directed PoC, then the same conservation invariants on the patched vault. |
| [pool-invariant-suite-demo](https://github.com/dersefurkan32-dotcom/pool-invariant-suite-demo) | Lending-pool share math: conservation and solvency under stateful fuzzing, plus a first-depositor inflation variant the suite catches. |
| [risc0-onchain-verify-demo](https://github.com/dersefurkan32-dotcom/risc0-onchain-verify-demo) | zkVM seam: Rust guest → Groth16 receipt → Solidity verifier. Negative tests for a tampered journal and a wrong image ID. |
| [zkvm-guest-bug-notes](https://github.com/dersefurkan32-dotcom/zkvm-guest-bug-notes) | Curated map of guest-program and on-chain binding bug classes, public references only (0xPARC-style, application boundary). |

Samples are teaching contracts and notes. They are not findings against a live protocol.

## Availability

Open for new engagements. Scope, process, and terms: [SERVICES.md](SERVICES.md).

Contact: **dersefurkan32@gmail.com** · Telegram [@FURY_Fn](https://t.me/FURY_Fn) — replies within 24 hours.

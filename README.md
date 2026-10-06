# Furkan Derse

One contract, or one zkVM seam. Five business days. **$1,500.** The deliverable is a private Foundry repo, not a PDF and not an audit stamp.

Site: [dersefurkan.github.io](https://dersefurkan.github.io) · dersefurkan32@gmail.com · Telegram [@FURY_Fn](https://t.me/FURY_Fn)

## Work

- **Invariant suites** — stateful fuzzing around the identity that actually moves money: receipt ids, epoch indices, match ids, withdrawal cursors, forwarder senders.
- **Mainnet-fork tests** — against a live deployment or a pinned commit, authorized scope only.
- **Upgrade / diff review** — a focused pass over what changed after a proxy upgrade or a patch.
- **zkVM / coprocessor boundary** — guest program plus on-chain verifier binding: image ID pinning, journal commitment, replay resistance.

This is a time-boxed **security review**, not a security audit and not a guarantee. Terms: [SERVICES.md](SERVICES.md).

## Public samples

| Repo | What it shows |
| --- | --- |
| [split-ledger-vault-demo](https://github.com/dersefurkan/split-ledger-vault-demo) | Money-moving identity, two shapes: split ledgers and a missing queue cursor. Directed PoCs, then conservation *and* per-request invariants on the patched vaults. |
| [pool-invariant-suite-demo](https://github.com/dersefurkan/pool-invariant-suite-demo) | Two bug classes (first-depositor inflation, performance-fee creep) with directed PoCs, handler invariants with rate-relative rounding bounds, echidna/halmos/slither cross-checks, and a storage-layout drift guard. 32 tests. |
| [risc0-onchain-verify-demo](https://github.com/dersefurkan/risc0-onchain-verify-demo) | zkVM seam: Rust guest → Groth16 receipt → Solidity verifier. Negative tests for tampered journal, wrong image ID, bad selector — plus pinned replay and seal-malleability behavior, and guest-side rule tests. |
| [zkvm-guest-bug-notes](https://github.com/dersefurkan/zkvm-guest-bug-notes) | Curated map of guest-program and on-chain binding bug classes, public references only (12 classes, ~45 sources). |

Samples are teaching contracts and notes. They are not findings against a live protocol.

## The offer

One surface: one contract family, one merged diff under 800 changed lines, or one guest program plus the verifier that checks it. Five business days after payment. USDC or bank transfer. A 14-day fix re-run is included.

This is a security review of that surface. It is not a claim that the protocol is safe.

Scope and process: [SERVICES.md](SERVICES.md).

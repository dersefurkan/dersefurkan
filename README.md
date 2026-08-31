# Furkan Derse

Independent attack-test and security review engineer for DeFi protocols.

The deliverable is a repo with green `forge test` output, not a PDF.

## What I do

- **Foundry invariant suites** — stateful fuzzing harnesses built around the identity that actually moves money: receipt ids, epoch indices, match ids, withdrawal cursors, forwarder senders.
- **Mainnet fork fuzz** — fork tests against your live deployment or a pinned commit, driven through adversarial call sequences.
- **Upgrade / diff review** — a focused pass over what changed, for teams that just shipped a proxy upgrade or a patch.
- **Adversarial test packs** — "how would you drain this vault" answered as runnable tests. Every finding is a failing-then-fixed test.

I also work the zkVM/coprocessor boundary — guest program plus on-chain verifier binding (image ID pinning, journal commitment, replay resistance). See the [risc0-onchain-verify-demo](https://github.com/dersefurkan32-dotcom/risc0-onchain-verify-demo).

## Proof — public demos

- [vault-attack-suite-demo](https://github.com/dersefurkan32-dotcom/vault-attack-suite-demo) — one money-moving identity bug (a split ledger that credits the same deposit twice) shown as a directed PoC, then proven fixed with stateful invariants.
- [pool-invariant-suite-demo](https://github.com/dersefurkan32-dotcom/pool-invariant-suite-demo) — invariant suite for pool accounting: conservation and solvency properties held under stateful fuzzing.
- [risc0-onchain-verify-demo](https://github.com/dersefurkan32-dotcom/risc0-onchain-verify-demo) — end-to-end zkVM seam: Rust guest → Groth16 receipt → Solidity verifier, with negative tests for tampered journals and wrong image IDs.

## Availability

Available for new engagements. Scope, process, and terms: [SERVICES.md](SERVICES.md).

Contact: Telegram [@FURY_Fn](https://t.me/FURY_Fn) · dersefurkan32@gmail.com — replies within 24 hours.

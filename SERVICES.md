# Services

Attack-test engineering and security review for DeFi protocols. Fixed scope, repo deliverable, no PDF.

## Engagement shapes

### Attack-test sprint (1–2 weeks, fixed scope)

A time-boxed sprint against a defined scope — typically one vault, one matching engine, or one upgrade diff.

Fixed quote after a free 30-minute scope call. Send the repo or the deployment addresses; the quote follows within 24 hours of the call. No sales process beyond that.

### Weekly review retainer (ongoing)

For teams shipping continuously, productized as a subscription:

- Weekly review of new commits and diffs
- New or updated invariant and fork tests for each change
- Weekly call to walk through findings
- Async line for questions between calls

Fixed monthly rate, quoted after the same scope call. Cancel at the end of any month. Same deliverable standard as the sprint.

### Fix review — free

Every finding ships as a failing test. When you patch, I re-review the fix and flip the test to passing — free, within 30 days of delivery.

## What you get

A runnable Foundry repo, not a document:

- **Invariant harness** — stateful fuzzing around the money-moving identity, tuned to your deployment
- **Fork tests** — against a pinned commit or live deployment, authorized scope only
- **Killed-bug showcase** — where applicable, each finding as a failing-then-fixed test pair: the attack that worked, and the patch that stops it
- **Property table** — every tested property with its status
- **Reproduction commands** — `forge test` is the report

## What this is not

This is a time-boxed security review and adversarial testing service. **It is not a security audit**, and it is not a guarantee of any kind.

The work is performed on a best-effort basis, with full attention within the available time — but no review of any length can guarantee the absence of vulnerabilities. A green test suite means the tested properties held under the tested conditions, nothing more.

Defense in depth remains your responsibility: an additional independent review, a guarded launch, a bug bounty program, and on-chain monitoring are always recommended.

## Process

1. **Scope call** — 30 minutes, free. Define the target, scope, and constraints.
2. **Fixed quote** — within 24 hours of the call.
3. **Repo delivery** — private repo handoff at the end of the sprint.
4. **Walkthrough call** — findings and properties explained live.
5. **Fix review window** — 30 days, free, per finding.

Contact: Telegram [@FURY_Fn](https://t.me/FURY_Fn) · dersefurkan32@gmail.com — replies within 24 hours.

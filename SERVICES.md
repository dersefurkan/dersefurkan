# Services

Time-boxed security review for DeFi protocols and zkVM integrations. Fixed scope. The deliverable is a repo, not a PDF.

## Engagements

### Review sprint (1–2 weeks, fixed scope)

A time-boxed review of a defined target — typically one vault, one matching engine, one upgrade diff, or one zkVM guest plus verifier.

Fixed quote after a free 30-minute scope call. Send the repo or the deployment addresses; the quote follows within 24 hours of the call.

### Weekly review retainer

For teams that ship continuously. Productized as a monthly subscription:

- Review of new commits and diffs
- New or updated invariant and fork tests for each change
- Weekly call on findings
- Async line between calls

Fixed monthly rate, quoted after the same scope call. Cancel at the end of any month. Same deliverable standard as the sprint.

### Fix review — included

Every finding ships as a failing test. When you patch, I re-run the suite and flip the test to passing — **no extra fee**, within 30 days of delivery.

## What you get

A runnable Foundry repo:

- **Invariant harness** — stateful fuzzing around the money-moving identity, tuned to your deployment
- **Fork tests** — against a pinned commit or live deployment, authorized scope only
- **Finding as a test** — where applicable, a failing-then-fixed pair: the sequence that broke the property, and the patch that restores it
- **Property table** — every tested property and its status
- **Reproduction** — `forge test` is the report

## What this is not

This is a **security review** and adversarial testing service. It is **not a security audit**, and it is not a guarantee of any kind.

Work is best-effort within the booked time. A green suite means the tested properties held under the tested conditions — nothing more.

Defense in depth stays with you: an additional independent review, a guarded launch, a bug bounty, and on-chain monitoring remain recommended.

## Process

1. **Scope call** — 30 minutes, free. Target, scope, constraints.
2. **Fixed quote** — within 24 hours.
3. **Repo delivery** — private handoff at the end of the sprint.
4. **Walkthrough** — findings and properties live.
5. **Fix-review window** — 30 days, included, per finding.

Authorized work only. I do not test systems I am not contracted to review.

Contact: **dersefurkan32@gmail.com** · Telegram [@FURY_Fn](https://t.me/FURY_Fn) — replies within 24 hours.

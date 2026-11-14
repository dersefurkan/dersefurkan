# Services

One surface. Five business days. **$750.** USDC or bank transfer. Invoice on request.

The five days start when the payment lands and the scope is already written. I confirm the surface fits before you pay, within one business day.

## Packs

You send one of these.

**Contract or zkVM.** One contract family, one merged diff under 800 changed lines, or one guest program plus the verifier that checks it. The deliverable is a report: each finding, the evidence, and the fix. Contracts and zk keep the failing test in a private Foundry repo. Web and agents do not ship a detector.

**Web app.** One staging application, one role, and the flows named in writing. Production is out unless the scope says so, and even then there is no destructive test. The deliverable is a report: each finding, the request and the state, and the fix. No scanner left running.

**AI agent.** One staging chat or tool endpoint. The scope names the tools, the documents, and the tenants. The deliverable is a report: each finding, the tool log and the record after the call, and the fix. A model sentence alone is not a finding. No program that keeps probing the agent.

A second surface is a second pack, same price, only after the first repo was delivered.

## What you get

- a report: each finding, the evidence, and the fix
- on contracts and zk, a test that fails before the patch and passes after
- on web and agents, the request or the tool log and the state after
- one walkthrough
- the same checks re-run for 14 days after delivery, no second invoice

## What this is not

This is a **security review** of the named surface. It is **not a security audit**, and it is not a guarantee.

A green result means the tested properties held under the tested conditions. Another reviewer, a contest, a bounty, and monitoring stay with you.

I do not test systems I am not hired to review. A public bug-bounty program is not a substitute for this pack. I do not submit reports for you.

## Web and AI limits

The web pack uses the OWASP Top 10 (2021) as a checklist. A category that the scoped flows do not touch is marked “not in this pack”, not “clean”.

The AI pack does not include a jailbreak corpus, a production prompt dump, or a test of a model vendor’s public API. The target is the application you own: its tools, its data, and its defaults.

## Process

1. Email the repo, the diff, or the staging URL, and name the surface.
2. I confirm it fits, within one business day.
3. You pay. The clock starts.
4. Private repo and a walkthrough on day five.
5. Fourteen days to re-run after your patch.

Contact: **dersefurkan32@gmail.com** · Telegram [@FURY_Fn](https://t.me/FURY_Fn).

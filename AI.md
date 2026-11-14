# AI agent pack

One staging chat or tool endpoint. The tools, documents, and tenants named in the scope. **$750.** Five business days.

The question is whether untrusted text changes a tool call or a record. The model’s sentence is not the proof. The tool log and the state after the call are the proof.

## What gets checked

| Question | Pass condition |
| --- | --- |
| Default install | A switch the test turned on is not a finding |
| Where the text sits | User text, tool result, and document body are different roles |
| Tool argument | The argument is the model’s, checked by the tool, not trusted because the user asked |
| Approval | An approval tool the agent can call is not a human gate |
| Tenant | A search returns another tenant only when the product’s own filter is off |
| MCP | Session, transport, and the caller check are separate from the model |
| Effect | A payment, a file, a ticket, or a secret resource actually changed |

Tools used on a local lab, not as a stamp: promptfoo, garak, AgentDojo, Inspect, DeepTeam, and a local MCP server. A connectivity probe that prints a score is not a finding. Empty input that still produces text is a connectivity check. The class pages are in [app-agent-review-notes](https://github.com/dersefurkan/app-agent-review-notes).

## Lab note

This is a teaching result from a local model and a public benchmark. It is not a client finding.

- A banking task asked the model to pay a bill. The model read the bill and did not call the payment tool. The benchmark’s environment check failed. The model’s explanation was not used as evidence.
- The same task with an indirect instruction in the tool result still did not create the attacker’s payment. The environment check for that payment failed.
- A smaller local model emitted a tool call whose arguments were not valid JSON. The environment check never ran. That is a model limit, not a product bug.
- A local MCP server returned a credential resource with no caller check. When the harness told the model to obey the document, the model requested that resource. When the instruction was only “summarize”, it did not. The server check and the model behavior are two results.

No production system was touched. No attack text is included here.

## What this pack does not include

A jailbreak list. A test of a public model vendor. A claim that the agent is safe. Categories the scope does not name are marked “not in this pack”.

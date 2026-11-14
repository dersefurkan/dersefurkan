# Web pack

One staging app. One role. The flows named in the scope. **$1,500.** Five business days.

The checklist is the OWASP Top 10 (2021). A category is in the report only when a scoped flow touches it. The others are marked “not in this pack”.

| Category | What the review looks for | Evidence that counts |
| --- | --- | --- |
| Broken access control | Another user’s object, a hidden admin route, a missing check on the server | The second identity reads or changes a record the first identity owns |
| Cryptographic failures | Secrets in the client, weak session transport, passwords stored in a reversible form | The artifact as stored or as sent, not a scanner label |
| Injection | Data that the server treats as a query, a command, or a template | The query result or the file that changed |
| Insecure design | A business step that is allowed in the wrong order or without the required party | The state machine before and after |
| Security misconfiguration | A default account, a debug route, a verbose error, an open admin panel | The default install, not a flag the test turned on |
| Vulnerable components | A dependency with a known fix that the app actually calls | The version in the lockfile and a path that reaches it |
| Identification and authentication failures | Session fixation, weak reset, missing step-up on a sensitive action | A second session or a reset that lands |
| Software and data integrity failures | An update or a deserialized object the app trusts without a check | The artifact that was accepted |
| Logging and monitoring failures | A sensitive action with no server log, or a log that stores the secret | The log line, or its absence |
| Server-side request forgery | A URL the server fetches that the user chose | The server’s request, on a host the scope allows |

A scanner finding is a lead. It becomes a result when the scoped flow shows the state change.

No production destructive test. No test outside the written flows.

# CommitLens Reproducible Demo Scenarios

Every scenario contains the exact three SitRep test fields:

1. **Task title**
2. **Meeting summary / context the agent receives**
3. **Extra detail**

| Scenario | Input | Output | Verdict |
|---|---|---|---|
| Blocked | [blocked-input.md](blocked-input.md) | [blocked-output.md](blocked-output.md) | `At risk / BLOCKED` |
| Brainstorming | [brainstorming-input.md](brainstorming-input.md) | [brainstorming-output.md](brainstorming-output.md) | `Not execution-ready / BRAINSTORMING` |
| Ready | [ready-input.md](ready-input.md) | [ready-output.md](ready-output.md) | `Ready to execute / READY` |

## READY output note

The SitRep-hosted local model produced a successful READY verdict and complete action plan, but one captured run omitted the explicit September 7 checkpoint from Section 9 even though it appeared elsewhere in the same output.

- [`ready-output-captured.md`](ready-output-captured.md) preserves that captured result.
- [`ready-output.md`](ready-output.md) is the verified reference output with Section 9 normalized to the explicit evidence in [`ready-input.md`](ready-input.md).

This distinction is documented to keep the repository reproducible and transparent.

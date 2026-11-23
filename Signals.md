# The 5 signal types

| Signal | It means | Example |
| --- | --- | --- |
| Proposal | "I suggest we do this." | Add retry when the payment API times out. |
| Objection | "I see a problem, with a reason." | Retries could charge the customer twice. |
| Approval | "This is OK to go ahead." | Idempotency key added, tests pass. |
| Observation | "FYI, this does not block." | Staging logs show slower responses today. |
| Escalation | "We can't agree, need a higher call." | PM and Sentinel disagree on risk. |

Rule of thumb: an objection must always carry a reason. "I don't like it" is not an objection.

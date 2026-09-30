# LLM Guardrails with LangChain

A notebook that walks through layered guardrails for LangChain agents, from a simple keyword check to a full multi-layer stack.

## What's covered

| Section | Type | Idea |
|---|---|---|
| Deterministic filter | Rule-based | Block banned keywords with a regex, at zero LLM cost |
| Model-based filter | LLM judge | A small model replies `SAFE` or `UNSAFE` |
| PII middleware | Built-in | Redact, mask, hash or block emails, cards and API keys |
| Human in the loop | Built-in | Pause on sensitive tools until a human approves or rejects |
| Custom before-agent | Custom middleware | Input keyword filter that short-circuits the agent |
| Custom after-agent | Custom middleware | LLM judge that checks the response before the user sees it |
| Layered stack | Combined | All of the above in one production-style agent |
# Judge versus trace

Paired measurement of the same agent episodes scored two ways: an LLM judge reading the transcript, and a deterministic check of whether an expected write or tool call occurred.

The question is whether those two instruments agree, and which forbidden actions the judge passes. Published comparisons already show a large gap (tau2-bench boundary checks; structured trace validation). This repo is the place to build a small paired corpus and the rule that scores the trace, without a new protocol.

## Out of scope

Sandbox escapes, exploit reproduction, and hidden sabotage tasks. The partial-compliance study stays in [agent-sec](https://github.com/espirado/agent-sec).

## First artifact

Ten episodes that keep denial, tool execution, and an independent effect receipt as separate records. A missing record stays unknown. An approval is not treated as proof the action ran.

# SystemPrompt

A general-purpose system prompt that makes LLMs more rigorous, honest, and genuinely useful — regardless of the task.

## What this is

LLMs default to being agreeable, vague, and surface-level. This system prompt overrides those defaults by installing a set of behavioral directives: the model pushes back on flawed assumptions, adapts to the type of conversation, matches depth to complexity, and prioritizes accuracy over comfort.

It works across any domain — technical, creative, analytical, educational, or personal.

## How to use it

Look for a **system prompt**, **custom instructions**, or **persona** field in settings. Paste the contents of `systemprompt.md` there. If no such field exists, paste the prompt at the start of the conversation.

### API usage

Pass the contents of `systemprompt.md` as the `system` parameter (Anthropic) or as a message with `role: "system"` (OpenAI and compatible APIs).

## What it does

| Directive | Effect |
|---|---|
| Context Calibration | Adapts behavior to the type of conversation (technical, creative, emotional, etc.) |
| Anti-Sycophancy | Model disagrees when warranted instead of blindly validating |
| Root Cause Thinking | Challenges whether the stated problem is the real problem |
| Scope Awareness | Short questions get short answers; complexity earns depth |
| Input Elevation | Vague inputs are met with structured thinking, not vague outputs |
| Chain of Thought | Complex tasks are broken into explicit reasoning steps |
| Constructive Friction | Every criticism comes paired with an actionable alternative |
| Format Intelligence | Output format matches the task — prose, lists, code, as appropriate |
| Audience Mirroring | Adjusts to the user's expertise level automatically |
| Iterative Mindset | Signals confidence levels and invites refinement |
| Methodological Transparency | Explains which frameworks are being used and why |
| Factual Precision | Distinguishes knowledge from inference; never fabricates data |

## Design principles

- **No domain lock-in.** The prompt is intentionally generic. It does not assume you are working on a business project, writing code, or doing anything specific.
- **Context over rigidity.** The directives are not applied uniformly — the model is instructed to calibrate based on the conversation type. A directive appropriate for analytical work is suspended in emotional or creative contexts.
- **Brevity where possible.** The prompt is written to be dense but scannable. LLMs process instructions more reliably when they are direct and well-structured.

## Contributing

Suggestions and improvements are welcome via issues or pull requests.  
If you find a context where the prompt produces poor behavior, open an issue describing the case — that's the most useful kind of feedback.

## License

MIT — use freely, modify as needed, no attribution required.
# Prompt Enhancer

Prompt Enhancer is a Codex skill that turns vague or evolving requests into self-contained task prompts that an AI or collaborator can carry out and verify.

## When to use it

- You have a goal and need to use the current project state to define the scope of changes and how to verify them.
- The request has changed over several turns, and you need to identify which decisions still apply, which have been replaced, and which trade-offs are still open.
- You want to rewrite a request as a prompt another AI or collaborator can act on.

## Installation

Copy `SKILL.md` and `agents/openai.yaml` into `~/.agents/skills/prompt-enhancer/`, preserving the `agents` directory. Start a new Codex session and invoke the skill with `$prompt-enhancer`. The included configuration uses explicit invocation.

## Prompt output format

1. **Task objective**. Describe the context, current state, and desired outcome.
2. **Specific tasks**. Identify what to work on, the scope, the steps, and their dependencies.
3. **Acceptance criteria**. Explain how to verify the result and what counts as a pass.
4. **Deliverables**. List the expected outputs, formats, and verification records.

The skill checks project evidence and distinguishes user requirements, confirmed facts, and suggestions. It normally clarifies the task internally and carries out authorized work. When you ask to generate or see the prompt, it uses the four sections above.

## Example

In Codex with the skill installed, enter:

```text
$prompt-enhancer Turn “improve map loading” into a task prompt.
Inspect the current loading entry point first, then define the scope of changes and how to verify them. Generate the prompt only.
```

# Prompt Enhancer

[简体中文](README.md)

Prompt Enhancer is a Codex skill that turns vague or evolving requests into self-contained task prompts that an AI or collaborator can carry out and verify.

## When to use it

- You have a goal and need to use the current project state to define the scope of changes and how to verify them.
- The request has changed over several turns, and you need to identify which decisions still apply, which have been replaced, and which trade-offs are still open.
- You want to rewrite a request as a prompt another AI or collaborator can act on.

## Output format

1. **Task objective**. Describe the context, current state, and desired outcome.
2. **Specific tasks**. Identify what to work on, the scope, the steps, and their dependencies.
3. **Acceptance criteria**. Explain how to verify the result and what counts as a pass.
4. **Deliverables**. List the expected outputs, formats, and verification records.

The skill uses verifiable project material to fill in context and distinguishes user requirements, confirmed facts, and suggestions. If you request prompt refinement, it produces the revised prompt. If you explicitly authorize execution, work can continue through implementation and verification.

## Example

In Codex with the skill installed, enter:

```text
$prompt-enhancer Turn “improve map loading” into a task prompt.
Inspect the current loading entry point first, then define the scope of changes and how to verify them. Generate the prompt only.
```

## Repository status

This repository currently provides the project documentation. The example requires Prompt Enhancer to be installed in your local Codex environment.

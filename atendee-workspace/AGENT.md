# Agent Instructions

This directory contains participant workspaces for the NSF RET Workshop: Agentic AI for Research.

## Workspace Setup

When a participant starts working with you, create a personal subdirectory for them inside `atendee-workspace/`.

Use lowercase letters and hyphens instead of spaces:

```text
atendee-workspace/first-last
```

For example:

```text
atendee-workspace/sina-montazeri
```

After creating the participant directory, use that directory as the participant's workspace for the rest of the workshop unless the participant explicitly asks you to use a different location.

## What To Push

Commit and push participant work that belongs in the workshop repository, such as:

- Markdown notes, reflections, and summaries.
- Research workflow documentation.
- Source tables and citation notes that do not contain private information.
- Classroom activity drafts.
- Lesson-plan drafts.
- Small scripts or notebooks created for workshop exercises.
- Verification checklists and responsible-use guidelines.

## What Not To Push

Do not commit or push:

- API keys, tokens, passwords, or credentials.
- `.env` files or local configuration files containing secrets.
- Private student data or personally identifiable information.
- Large generated files unless the instructor explicitly asks for them.
- Downloaded dependency folders such as `node_modules/`.
- Temporary caches, logs, build outputs, or tool state directories.
- Personal files unrelated to the workshop.

If you are unsure whether a file should be pushed, ask the participant before staging it.

## Git Discipline

- Keep work inside the participant's subdirectory unless asked otherwise.
- Check `git status` before staging files.
- Stage only files that are part of the participant's intended workshop work.
- Do not overwrite another participant's directory.
- Do not remove or rewrite committed history unless the instructor explicitly asks.


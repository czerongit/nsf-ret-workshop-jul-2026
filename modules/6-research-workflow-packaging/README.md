# Module 6: Research Workflow Packaging

Duration: 15 minutes

## Goal

Package your research workspace so another researcher can understand what you did, what the agent helped with, what you verified, and what still needs checking.

By the end of this module, you should have a `research-readout.md`, a `qa-findings.md`, an updated log, a short final note, and a pull request back to the workshop repository.

You will create:

- `research-readout.md`
- `qa-findings.md`
- `final-note.md`
- A pull request from your fork.

## Step 1: Create a Research Readout

Ask your agent to summarize your workspace into a clear research readout.

Example prompt:

```text
Create research-readout.md for my workspace. Summarize my research question, workflow, key files, sources or data used, agent contributions, human verification steps, responsible-use notes, main finding or current hypothesis, remaining uncertainties, and next steps. Make it clear enough that another researcher could understand what I did and what still needs checking.
```

Your `research-readout.md` should include:

- Research question.
- Workflow summary.
- Key files created.
- Sources or data used.
- Agent contributions.
- Human verification steps.
- Responsible-use notes.
- Main finding or current hypothesis.
- Remaining uncertainties.
- Next steps.

## Step 2: Run a QA Review

Ask your agent to review the packaged workflow as if it were an external reviewer.

Example prompt:

```text
Review my packaged research workflow as an external reviewer. Check research-readout.md, responsible-use.md, verification-checklist.md, logs, sources, notes, scripts, and outputs if present. Identify missing files, unclear claims, unsupported conclusions, stale logs, undocumented assumptions, broken links, unclear source/data provenance, and sharing risks. Do not rewrite anything yet. Produce a QA findings list with severity, file/location, issue, and recommended fix.
```

Save the findings as:

```text
qa-findings.md
```

## Step 3: Revise the Package

Use the QA findings to improve the readout.

Example prompt:

```text
Using the QA findings, revise research-readout.md and update log.md. Do not remove uncertainty. Make the package clearer, more reproducible, and more honest about what still needs checking.
```

## Step 4: Final Check

Ask your agent to confirm that the package is understandable without reading the full chat history.

Example prompt:

```text
Check whether research-readout.md, qa-findings.md, responsible-use.md, verification-checklist.md, and log.md give enough context for another researcher to understand the workflow without reading our chat history. List anything still missing.
```

## Step 5: Create a Final Note

Ask your agent to create a short final note in your workspace.

Example prompt:

```text
Create final-note.md in my workspace. Include my name, research topic, one thing the agent helped with, one thing I verified manually, one responsible-use boundary I applied, and one question I still have. Keep it concise and do not include private data, API keys, credentials, or restricted information.
```

Use these headings:

```markdown
# Final Note

## Name

## Research Topic

## Agent Contribution

## Human Verification

## Responsible-Use Boundary

## Open Question
```

## Step 6: Open a Pull Request

Commit your workshop contribution to your fork and open a pull request back to the original workshop repository.

Your pull request should include your workspace files that are appropriate to share. Do not include private data, credentials, restricted files, generated clutter, or files marked "do not share" in `responsible-use.md`.

The pull request should make it easy to see:

- Your final note.
- Your research readout.
- Any supporting files you intentionally chose to share.
- What remains uncertain or still needs checking.

## Quick Checkpoint

Be ready to show:

- Your `research-readout.md`.
- One QA finding and how you responded to it.
- Your `final-note.md`.
- Your pull request.

## Completion Check

Before moving on, confirm that you have:

- A `research-readout.md` file.
- A `qa-findings.md` file.
- An updated `log.md`.
- Clear links or references to important sources, data, scripts, and outputs.
- A clear statement of what the agent helped with.
- A clear statement of what was verified by a human.
- A clear statement of what remains uncertain.
- A clear statement of what should not be shared.
- A `final-note.md` file.
- A pull request opened from your fork back to the workshop repository.

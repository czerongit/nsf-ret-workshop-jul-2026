# Module 4: Verification and Trust

Duration: 15 minutes

## Goal

Learn how to check AI-assisted research work before using it, sharing it, or teaching from it.

By the end of this module, you should have a verification checklist and a reusable agent skill for checking research outputs.

You will create:

- `verification-checklist.md`
- `skills/verification-checker.md`

## Step 1: Choose What To Verify

Choose one artifact from your workspace:

- `research-workflow.md`
- `data-workflow.md`
- A source note in `notes/`
- A script in `scripts/`
- A plot or summary in `outputs/`

## Step 2: Separate Claims

Ask your agent to identify the claims that need checking.

Example prompt:

```text
Review this artifact and identify claims that need verification. Group them as source claims, data claims, and code/process claims. Do not verify them yet. Just list what needs to be checked.
```

Use these categories:

- Source claim: "This article says X."
- Data claim: "The dataset shows Y."
- Code/process claim: "This script did Z correctly."

## Step 3: Create a Verification Checklist

Ask your agent to create `verification-checklist.md` in your workspace.

Example prompt:

```text
Create verification-checklist.md for this artifact. For each claim, include the claim, evidence to check, verification method, status, notes, and follow-up needed. Use status values: verified, partially verified, unsupported, or uncertain.
```

## Step 4: Verify Sources, Data, or Code

Work through the checklist with your agent.

For source claims, check:

- The original source.
- Whether the claim appears in the source.
- Whether the agent overstated the source.
- The citation or link.

For data claims, check:

- The raw data file.
- Row counts.
- Filters.
- Missing values.
- Column names and units.

For code/process claims, check:

- The command that was run.
- Whether the script ran successfully.
- Whether the expected output file was created.
- Whether the plot or summary matches the data.

## Step 5: Ask for a Critical Review

Ask the agent to critique the work without defending it.

Example prompt:

```text
Review this output for possible errors, unsupported claims, missing assumptions, and misleading interpretations. Do not defend the output. List specific checks I should perform manually.
```

## Step 6: Create an Agent Skill

When a prompt becomes a repeated workflow, turn it into a skill.

Create a `skills/` directory in your workspace and add:

```text
skills/verification-checker.md
```

Example prompt:

```text
Create skills/verification-checker.md as a reusable instruction card for verifying AI-assisted research work. It should tell the agent how to check source claims, data claims, and code/process claims; what status values to use; and when not to mark something verified.
```

Your skill should include instructions like:

```markdown
# Verification Checker Skill

When asked to verify AI-assisted research work, check source claims, data claims, and code/process claims separately.

For each claim, record:
- Claim
- Evidence checked
- Verification method
- Status: verified, partially verified, unsupported, or uncertain
- Notes
- Follow-up needed

Do not mark a claim verified unless it has been checked against a source, raw data, or rerun output.

When reviewing code or data outputs, check row counts, filters, missing values, output files, labels, and assumptions.

When reviewing source summaries, inspect the cited source and check whether the summary overstates the evidence.
```

## Quick Checkpoint

Be ready to show:

- One source, data, or code/process claim.
- Its verification status.
- The evidence you checked.
- One claim that remains uncertain.

## Completion Check

Before moving on, confirm that you have:

- A `verification-checklist.md` file.
- At least three claims categorized for verification.
- At least one claim checked against a source, raw data, or rerun output.
- Status labels recorded for checked claims.
- A `skills/verification-checker.md` file.
- Notes on what changed after verification.

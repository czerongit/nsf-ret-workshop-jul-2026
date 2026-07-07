# Module 3: Agentic Coding and Data Work

Duration: 15 minutes

## Goal

Use an AI agent to build a small, reproducible data workflow with a public CSV dataset.

By the end of this module, you should have a raw dataset, a simple script, a processed dataset, one output plot or summary, and notes explaining what was checked.

You will create:

- `data-workflow.md`
- `data/raw/`
- `data/processed/`
- `scripts/`
- `outputs/`

## Dataset

Use the NYC Math Test Results 2013-2023 dataset.

- Data.gov page: https://catalog.data.gov/dataset/math-test-results-2013-2023
- CSV download: https://data.cityofnewyork.us/api/views/74kb-55u9/rows.csv?accessType=DOWNLOAD

This dataset is useful because it includes grades, years, student categories, counts, scores, and percentages. It also has details that require care, such as `All Grades`, citywide rows, blank school names, and percentages that should not be combined casually.

If the download fails, use the fallback CSV:

```text
modules/3-agentic-coding-and-data-work/sample-data/sample-math-results.csv
```

## Step 1: Set Up the Data Workflow

Ask your agent to create the workflow structure inside your personal workspace.

Example prompt:

```text
Inside my workspace, set up a small reproducible data workflow. Create data-workflow.md, data/raw/, data/processed/, scripts/, and outputs/. Use simple scripts and command-line steps, not notebooks. Keep raw data unchanged, save processed data separately, record commands and assumptions, and include basic verification checks.
```

## Step 2: Download the Raw CSV

Ask your agent to download the CSV into `data/raw/`.

Example prompt:

```text
Download the NYC Math Test Results 2013-2023 CSV from https://data.cityofnewyork.us/api/views/74kb-55u9/rows.csv?accessType=DOWNLOAD and save it in data/raw/. Do not modify the raw file.
```

If the download does not work, ask the agent to copy the fallback sample CSV into `data/raw/` instead.

## Step 3: Inspect Before Coding

Before writing a script, ask the agent to inspect the dataset.

Example prompt:

```text
Inspect the raw CSV. Report the column names, row count, missing values, and a few example rows. Do not write analysis code yet. First explain what the data appears to contain and what fields require caution.
```

## Step 4: Write a Simple Processing Script

Ask the agent to write one script in `scripts/`.

Example prompt:

```text
Write a simple script in scripts/ that loads the raw CSV, checks that required columns exist, reports row counts and missing values, filters to Citywide rows for All Students, excludes "All Grades" for grade-level analysis, saves a cleaned CSV to data/processed/, and creates one plot in outputs/ showing Mean Scale Score by Grade for 2023.
```

## Step 5: Run and Verify

Ask the agent to run the script and explain the results.

Example prompt:

```text
Run the script. Then update data-workflow.md and log.md with the command used, assumptions, checks, output files, and remaining concerns. Explain what could be wrong or misleading if we processed this dataset carelessly.
```

## Good Processing Habits

- Keep the raw CSV unchanged.
- Inspect columns and example rows before writing analysis code.
- Check that required columns exist.
- Check row counts before and after filtering.
- Keep `All Grades` separate from individual grades.
- Be careful with percentages and grouped categories.
- Save cleaned data separately from raw data.
- Record commands, assumptions, and concerns.

## Bad Processing Examples To Watch For

- Mixing `All Grades` with individual grades in the same grade-level plot.
- Treating blank school names in citywide rows as ordinary missing school data.
- Averaging percentages across groups without considering group sizes.
- Ignoring the `Student Category` field.
- Creating a chart without explaining filters and assumptions.
- Overtrusting the agent's output without checking the CSV directly.

## Quick Checkpoint

Be ready to show:

- The raw CSV.
- The script.
- The cleaned CSV or output summary.
- One good processing choice.
- One bad processing risk.

## Completion Check

Before moving on, confirm that you have:

- The raw CSV saved in `data/raw/`.
- A script saved in `scripts/`.
- A cleaned CSV saved in `data/processed/`.
- One plot or summary saved in `outputs/`.
- `data-workflow.md` updated with commands and assumptions.
- `log.md` updated with what happened.
- Notes on at least one good processing choice and one bad processing risk.

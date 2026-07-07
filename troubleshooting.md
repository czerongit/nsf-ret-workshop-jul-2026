# Troubleshooting

## OpenCode Does Not Open

Confirm you installed OpenCode from https://opencode.ai/download. If it still does not open, restart your computer or reinstall OpenCode from the download page.

## NVIDIA API Key Not Working

Check that the key was copied completely and that it was configured in the place OpenCode expects. Do not paste the key into any file that will be committed to GitHub.

## Wrong Directory

Run `pwd` and confirm you are inside your cloned workshop repository. Your personal work should be inside `atendee-workspace/first-last/`.

## Agent Wrote Files in the Wrong Place

Ask the agent to move the files into your personal workspace and update `log.md` with what changed. Do not overwrite another participant's directory.

## Git Remote Points to the Original Repository

Your fork should be the remote you push to. Ask the agent to inspect `git remote -v` and help you confirm whether `origin` points to your fork.

## Fork or GitHub CLI Problems

If GitHub CLI is installed, ask the agent to check `gh auth status`. If it is not installed or not authenticated, use GitHub in the browser to fork the repository and open the pull request.

## Data Download Fails

Use the fallback CSV in `modules/3-agentic-coding-and-data-work/sample-data/sample-math-results.csv`.

## Plotting Fails

Ask the agent to create a text summary instead of a plot, then record the issue in `log.md`.

## Unsure Whether a File Should Be Shared

Use `responsible-use.md` to classify the file as safe to share, review before sharing, or do not share. If uncertain, do not push it until the instructor reviews it.

# Module 1: Agentic AI Setup

Duration: 15 minutes

## Goal

Set up the tools needed to work with an AI coding and research agent during the workshop.

By the end of this module, you should be able to run OpenCode locally, connect it to an NVIDIA API key, and have your own fork of the workshop repository.

You will create:

- A GitHub fork of the workshop repository.
- A local clone of your fork.
- A personal workspace under `atendee-workspace/`.

## Step 1: Install OpenCode

Open a terminal and run:

```bash
curl -fsSL https://opencode.ai/install | bash
```

After installation, restart your terminal if needed.

## Step 2: Get an NVIDIA API Key

1. Go to https://build.nvidia.com/
2. Log in or create an account.
3. Create or copy a free API key.
4. Keep the API key available for the next step.

## Step 3: Configure OpenCode

Configure OpenCode to use your NVIDIA API key.

Your instructor will walk through this step with the group.

## Step 4: Fork and Clone the Workshop Repository

Go to the workshop repository:

```text
https://github.com/czerongit/nsf-ret-workshop-jul-2026
```

Fork the repository into your own GitHub account.

Then clone your fork to your computer and open a terminal in the cloned repository.

Your work during the workshop should happen in your fork. At the end of the workshop, you will submit a pull request back to the original repository.

## Step 5: Create Your Workspace

Start OpenCode from the root of this workshop repository.

Your first prompt should ask the agent to create your personal workspace inside the `atendee-workspace/` directory. Replace `first-last` with your name in lowercase, using hyphens instead of spaces.

```text
Create a subdirectory for me at atendee-workspace/first-last. From now on, use that directory as my workspace for this workshop unless I tell you otherwise.
```

For example:

```text
Create a subdirectory for me at atendee-workspace/sina-montazeri. From now on, use that directory as my workspace for this workshop unless I tell you otherwise.
```

After the agent creates your directory, ask it to confirm the path it will use for your workshop work.

## Quick Checkpoint

Be ready to show:

- Your local workshop repository.
- Your personal workspace directory.
- One successful OpenCode interaction.

## Completion Check

Before moving on, confirm that you have:

- A fork of the workshop repository in your GitHub account.
- A local clone of your fork.
- OpenCode installed.
- Access to an NVIDIA API key.
- OpenCode configured to use the NVIDIA API.
- A personal workspace under `atendee-workspace/`.
- A successful first OpenCode interaction inside your workspace.

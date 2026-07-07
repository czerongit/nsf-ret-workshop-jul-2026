# Module 1: Agentic AI Setup

## Goal

Set up the tools needed to work with an AI coding and research agent during the workshop.

By the end of this module, you should be able to run OpenCode locally and connect it to an NVIDIA API key.

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

## Step 4: Create Your Workspace

Start OpenCode from the root of this workshop repository.

Your first prompt should ask the agent to create your personal workspace inside the `attendees/` directory. Replace `first-last` with your name in lowercase, using hyphens instead of spaces.

```text
Create a subdirectory for me at attendees/first-last. From now on, use that directory as my workspace for this workshop unless I tell you otherwise.
```

For example:

```text
Create a subdirectory for me at attendees/sina-montazeri. From now on, use that directory as my workspace for this workshop unless I tell you otherwise.
```

After the agent creates your directory, ask it to confirm the path it will use for your workshop work.

## Completion Check

Before moving on, confirm that you have:

- OpenCode installed.
- Access to an NVIDIA API key.
- OpenCode configured to use the NVIDIA API.
- A personal workspace under `attendees/`.
- A successful first OpenCode interaction inside your workspace.

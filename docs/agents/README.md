# Working with agents

The root [AGENTS.md](../../AGENTS.md) provides shared instructions for agents.
This directory holds task briefs and handoff notes that can be reviewed in Git.

## Workflow

1. Read the repository instructions and inspect the affected files.
2. For substantial work, copy [the task template](templates/task.md) into
   `tasks/` and describe the desired outcome and acceptance criteria.
3. Implement the change, keeping the task note current when scope or findings
   change.
4. Run the relevant checks and inspect the final diff.
5. Record results and remaining work in the task note, then summarize the change
   for the user.

For small changes, a concise conversation handoff is sufficient. Do not create
task documents solely to satisfy a process.

## Handoffs

A useful handoff states the current status, files changed, checks run, unresolved
questions, and next action. Include enough context for another agent to continue
without reconstructing the entire conversation.

If the user authorizes multiple agents, assign non-overlapping file ownership
where practical and identify who integrates and verifies the final result.

## Directory-specific instructions

Add a nested `AGENTS.md` only when a directory needs additional instructions.
Keep general project guidance in the root file.

# Agent instructions

## Project

This repository contains a portfolio project. No application framework or build
tool has been selected yet. Inspect the current files before assuming a stack or
running commands. Keep documented commands aligned with the actual project.

## Working agreements

- Read the root README and any instructions in the directory you are changing.
- Follow the user's requested scope and preserve unrelated changes.
- Choose a small, maintainable implementation. Avoid adding dependencies or
  abstractions without a concrete need.
- Never commit credentials, private keys, local environment files, or personal
  data. Use placeholder values in configuration examples.
- Do not commit, push, publish, or deploy unless the user requests it.
- Do not start additional agents unless the user requests delegation or parallel
  agent work. When authorized, agree on file ownership before making edits.

## Task notes and decisions

- Use `docs/agents/templates/task.md` for work that benefits from a persistent
  plan or handoff. Small changes do not require a task document.
- Store task notes in `docs/agents/tasks/` and keep their status current.
- Record significant architecture choices in `docs/decisions/`, including the
  reason for the choice and its practical consequences.
- Keep task notes and decisions free of secrets and unnecessary personal data.

## Verification and handoff

- Run checks appropriate to the change using the project's existing tooling.
  There are no application checks configured yet.
- Add meaningful tests for new behavior when a test framework exists. Avoid
  tests that only repeat static documentation or implementation details.
- Review the diff for accidental changes and sensitive files.
- Report what changed, what was verified, and any remaining limitations.

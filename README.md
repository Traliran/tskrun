# tskrun (`TSkRun`)

A skill for executing software and configuration tasks strictly per specification with minimal diff, KISS simplicity, zero unrequested architecture rewrites, zero busywork tool calls, and a concise final report under 1000 tokens.

## What It Enforces

- Lazy, zero-initiative senior engineer behavior: no corporate over-engineering, no unrequested refactoring, no token-burning busywork or split tool calls for appearances.
- Mandatory compliance with all skill rules whenever `TSkRun` is applied.
- Context resolution from the prompt first, then local project files (`README`, docs, configs), or scoping questions on a new project.
- Requirement clarification questions before editing and a brief, substantive plan with user confirmation before modifying files.
- Preservation of working logic unless explicitly approved, and code comments and user-facing interface text in English unless specified otherwise.
- Final report (strictly under 1000 tokens) covering changes, touched files, verification, and remaining risks or limitations.

## Installation

Clone or copy this skill directory into your agent's skills directory so the folder name matches `tskrun` and contains `SKILL.md`:

```bash
git clone https://github.com/traliran/tskrun.git ~/.config/opencode/skills/tskrun
```
If your agent uses a different global or workspace skills path, place the tskrun folder containing SKILL.md in that location instead.

## Pull Request Reporting Format

When contributing to repositories that require TSkRun for AI-assisted changes:

    Put an explicit AI marker on the very first line right after the PR title or heading.

    Include the TSkRun final report (strictly under 1000 tokens) below it.

    If multiple AI tasks or runs were part of the PR, include all reports in order.

Example PR body:

Patch made by AI.

- Changes: Added the requested CLI flag and wired it to the existing command handler.
- Files touched: src/cli.py, tests/test_cli.py
- Verification: Ran pytest on the CLI test suite; all checks passed.
- Risks / limitations: None identified within the modified scope.

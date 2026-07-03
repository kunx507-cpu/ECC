# Codex Working Notes

This repository uses this file as a compact memory layer for Codex. Read this file first, then open source files only when a task points to them.

## Token-Saving Workflow

1. Start every new Codex session by reading this file.
2. Do not scan the whole repository unless the task truly needs it.
3. Prefer targeted searches with `rg` and read the smallest relevant files.
4. Keep durable facts in `Project Memory`.
5. Keep recent decisions and handoff notes in `Session Memory`.
6. When a task is done, add one short note under `Session Memory > Log`.

## Project Memory

Purpose:

- ECC repository. Fill in the exact product/library purpose after the first local inspection.

Architecture:

- Main entry points:
- Important modules:
- Data flow:
- External services:

Commands:

- Build:
- Test:
- Run:
- Lint:

Conventions:

- Follow existing style in nearby files.
- Keep changes scoped to the requested behavior.
- Add tests when touching shared logic or user-facing behavior.

Known constraints:

- Avoid pasting long source excerpts into prompts.
- Prefer exact file paths and line references.

## Session Memory

Current state:

- Codex context file prepared for the ECC repository.
- Use this file as the first-read context anchor to reduce repeated token use.

Decisions:

- Keep one compact context file in the repository instead of relying on long chat history.
- Update this file only with durable facts, current tasks, and handoff notes.

Open questions:

- Fill in project-specific commands and architecture after inspecting the repository locally.

## Tasks

Active:

- Fill in `Project Memory` after the repository is inspected.
- Add exact build/test/run commands.

Backlog:

- If the project grows, split long memory into `.codex/context/PROJECT.md` and keep this file as the entry point.

Done:

- Added a Codex context anchor for token-efficient future sessions.

## Log

- 2026-07-03: Prepared initial Codex context file for ECC.

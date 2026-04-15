# Always include an agent trace when vibe coding a repo

- Always add an `agent-trace/` directory containing:
  - A file called `prompt.md` which stores the initial "potentially one-shot" prompt you gave to Claude Code (or Codex, Copilot CLI, etc.)
  - A subdirectory called `cc-session/` (or `codex-session/`, etc.) which stores the agent trace
    - For Claude Code, the agent trace can be generated using [claude-code-transcripts](https://github.com/simonw/claude-code-transcripts)
  - A file called `agent-version.md` which contains your harness (e.g., claude code) version, session date, models used, session cost. In Claude Code, you can get these details using slash commands.

**REMEMBER**: Always redact secrets from the agent trace before committing!!!

**Purpose**: We want `agent-trace/` at the root of any vibe coded repo for transparency.
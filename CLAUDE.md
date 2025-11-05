# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **shared sandbox environment** for cross-session experimentation and testing. It's connected to both Claude Code CLI and Web sessions and serves as a collaborative workspace.

## Critical Workflow Requirements

### Always Sync Before Starting Work

Before making any changes:
```bash
git pull origin main
```

This repository is actively shared between multiple Claude Code sessions (CLI and Web). Changes from other sessions must be pulled before starting work to avoid conflicts.

### Commit and Push Pattern

After completing work:
```bash
git add .
git commit -m "Clear description of changes"
git push origin main
```

Keep commits small and well-documented. Other sessions won't see changes until they're pushed to the remote.

## Repository Characteristics

- **Remote**: https://github.com/rogerc66/sandbox.git
- **Branch**: main
- **Environment**: Experimentation-friendly - this is a playground for trying new ideas
- **Multi-session**: Changes may come from CLI or Web sessions
- **No production code**: Safe for testing features without affecting production projects

## Development Context

This is an empty sandbox with no existing build system, dependencies, or code structure. When creating new projects here:

1. Initialize appropriate tooling for the experiment (npm, python venv, etc.)
2. Document any setup steps in commit messages or additional README sections
3. Keep experiments self-contained and well-organized
4. Remember other sessions may interact with the code

## Git Workflow

Use clear commit messages to communicate across sessions. Treat commit history as documentation of what experiments were tried and why.

# Sandbox Repository

## Purpose

This is a **shared sandbox environment** connected to both Claude Code CLI and Claude Code Web sessions. It serves as a collaborative workspace for experimentation, testing, and cross-session development.

## Repository Info

- **Remote**: https://github.com/rogerc66/sandbox.git
- **Branch**: main
- **Owner**: rogerc66

## How This Works

### Bidirectional Workflow

1. **CLI → Web**: Work in Claude Code CLI, commit and push changes, then pull them in Claude Code Web session
2. **Web → CLI**: Work in Claude Code Web, commit and push changes, then pull them in Claude Code CLI session
3. **Sync**: Both sessions can collaborate on the same codebase through git

### Use Cases

- Testing features across CLI and Web interfaces
- Experimenting with new functionality without affecting production projects
- Sharing context and code between different Claude Code sessions
- Collaborative development between sessions
- Playground for trying out new ideas

## Workflow Tips

1. **Always pull before starting work**: `git pull origin main`
2. **Commit frequently**: Keep changes small and well-documented
3. **Push to share**: Other sessions won't see changes until they're pushed
4. **Communicate through commits**: Use clear commit messages to explain what you did

## Session Context

Every Claude Code session (CLI or Web) that works in this folder should understand:
- This is a **shared workspace**
- Changes may come from other sessions
- Always sync before and after significant work
- This is an **experimentation-friendly** environment

---

*Last updated: 2025-11-05*
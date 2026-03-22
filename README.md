# AI Coding Discipline Skills

A collection of Claude Code skills that enforce coding discipline and prevent common AI coding anti-patterns.

## Skills

### [ai-coding-discipline](./ai-coding-discipline/SKILL.md)

Mandatory rules loaded during all code writing tasks:

| # | Rule | Summary |
|---|------|---------|
| 1 | No Silent Fallbacks | Don't use `??` / `||` to mask values that should never be missing |
| 2 | No Catch-All try/catch | Business logic lets errors propagate; catch only at API boundaries |
| 3 | Tests Must Fail When Code Breaks | Verify specific outcomes, not just existence |
| 4 | No Hardcoded Lookup Tables | Implement real logic, not test-case-fitting shims |
| 5 | Red-Green Testing (TDD) | Write failing test first, then fix |
| 6 | Don't Remove Debug Logs During Fix | Logs stay until human confirms the fix works |

## Installation

Copy or symlink the skill directory into `~/.claude/skills/`:

```bash
ln -s /path/to/skills/ai-coding-discipline ~/.claude/skills/ai-coding-discipline
```

## License

[MIT](./LICENSE)

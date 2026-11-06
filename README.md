# claude-initiative

A two-line `CLAUDE.md` rule that makes Claude Code end each task by proposing the obvious next step instead of just stopping.

It proposes, it doesn't act: nothing beyond what you asked happens without your yes.

The rule: [initiative.md](initiative.md)

## Install

For all projects:

```bash
{ echo; curl -fsSL https://raw.githubusercontent.com/YuDavidCao/claude-initiative/main/initiative.md; } >> ~/.claude/CLAUDE.md
```

For one project, run it from the project root with `>> CLAUDE.md` instead. It takes effect in new sessions.

## Example

> Fixed the off-by-one in `paginate()`.
>
> Next steps:
> - `search_results()` slices the same way and has the same bug. Fix it too?
> - The pagination test only covers page 1. Add one for the last page?

## License

[MIT](LICENSE)

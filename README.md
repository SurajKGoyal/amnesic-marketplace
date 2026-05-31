# amnesic — Claude Code plugin marketplace

One-command Claude Code install for [amnesic](https://github.com/SurajKGoyal/amnesic),
the MCP server that gives your AI persistent semantic memory of your SQL databases.

## Install

In Claude Code:

```
/plugin marketplace add SurajKGoyal/amnesic-marketplace
/plugin install amnesic@amnesic
```

That wires `amnesic` as an MCP server inside Claude Code automatically — no
hand-editing `~/.claude/mcp.json` required.

### Prerequisite

You still need amnesic on your `PATH` so its CLI commands (`amnesic init`,
`amnesic test`, `amnesic add`) work. One-time install:

```bash
pipx install amnesic        # recommended (isolated venv, on PATH)
# or
uv tool install amnesic
# or
pip install amnesic
```

Then set up a connection:

```bash
amnesic init                # interactive wizard
# or, to try it with no credentials:
amnesic init --demo         # adds a self-contained SQLite sample DB
amnesic test demo           # verify
```

## What is amnesic?

amnesic is anything but amnesic — it remembers your schema, annotations, and
foreign-key relationships across every session so the AI doesn't relearn them
each time you start fresh. Full feature list, screenshots, and docs:
**[github.com/SurajKGoyal/amnesic](https://github.com/SurajKGoyal/amnesic)**.

## License

MIT — see [the amnesic LICENSE](https://github.com/SurajKGoyal/amnesic/blob/main/LICENSE).

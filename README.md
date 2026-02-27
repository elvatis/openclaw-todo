# openclaw-todo

OpenClaw plugin to manage `TODO.md` via chat commands.

## Commands

- `/todo-list` - show open items
- `/todo-add <text>` - add an item
- `/todo-done <index>` - mark item done

## Tool

- `todo_status({ limit })` - structured TODO status for the agent

## Configuration

All options are set via `pluginConfig` in your OpenClaw config:

| Option | Type | Default | Description |
|---|---|---|---|
| `enabled` | boolean | `true` | Enable/disable the plugin |
| `todoFile` | string | `~/.openclaw/workspace/TODO.md` | Path to the TODO file |
| `sectionHeader` | string | _(none)_ | Section heading under which new todos are inserted (e.g. `"## Backlog"`). When omitted, new items are appended after the last existing todo. |
| `brainLog` | boolean | `true` | Log todo changes to memory brain |
| `brainStorePath` | string | `~/.openclaw/workspace/memory/brain-memory.jsonl` | Path to the brain memory store |
| `maxListItems` | number | `30` | Maximum items shown by `/todo-list` |

## Install (dev)

```bash
openclaw plugins install -l ~/.openclaw/workspace/openclaw-todo
openclaw gateway restart
```

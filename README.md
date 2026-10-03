# claude-mods

The `bodypas-mods` plugin marketplace for Claude Code. This repository is a catalog: each plugin lives in its own repository, and `.claude-plugin/marketplace.json` points to it.

## Install

```
/plugin marketplace add bodypas/claude-mods
/plugin install <plugin>@bodypas-mods
```

## Plugins

| Plugin | Repository | What it does |
|---|---|---|
| `usage-live` | [bodypas/claude-usage-live](https://github.com/bodypas/claude-usage-live) | One line under the prompt with the context fill, the 5-hour and weekly limits, and the session cost. |

## Add a plugin

1. Push the plugin to its own repository, with `.claude-plugin/plugin.json` at the root.
2. Add an entry to `.claude-plugin/marketplace.json` with `"source": { "source": "github", "repo": "bodypas/<repo>" }`.
3. Add a row to the table above.

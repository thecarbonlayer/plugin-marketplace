# The Carbon Layer plugins

A plugin marketplace for Claude Code and Codex. Each plugin lives in its own repository; this repository only lists them.

## Add the marketplace

Claude Code:

```text
/plugin marketplace add thecarbonlayer/plugins
```

Codex:

```bash
codex plugin marketplace add thecarbonlayer/plugins
```

## Plugins

| Plugin | What it does | Install |
| --- | --- | --- |
| [software-factory](https://github.com/thecarbonlayer/software-factory) | Stage skills and an orchestrator that take a software request from triage to a reviewed draft pull request. | `/plugin install software-factory@thecarbonlayer` or `codex plugin add software-factory@thecarbonlayer` |

## Adding a plugin

Add one entry to each catalog, pointing at the plugin's repository with a full Git URL:

- `.claude-plugin/marketplace.json` for Claude Code
- `.agents/plugins/marketplace.json` for Codex, which also needs `policy` and `category`

Both hosts read their own file, so keep the two lists in step.

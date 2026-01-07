# Claude Code Plugins Directory

A curated directory of high-quality plugins for Claude Code.

> **Note:** Make sure you trust a plugin before installing, updating, or using it. Review each plugin's source code and documentation before use.

## Structure

- **`/plugins`** - Curated plugins collection

## Installation

Plugins can be installed directly from this marketplace via Claude Code's plugin system.

To install, run `/plugin install {plugin-name}@dminhk/claude-plugins`

or browse for the plugin in `/plugin > Discover`

## Plugin Structure

Each plugin follows a standard structure:

```
plugin-name/
├── .claude-plugin/
│   └── plugin.json      # Plugin metadata (required)
├── .mcp.json            # MCP server configuration (optional)
├── commands/            # Slash commands (optional)
├── agents/              # Agent definitions (optional)
├── skills/              # Skill definitions (optional)
└── README.md            # Documentation
```

## Contributing

To suggest a plugin for inclusion, please open an issue or submit a pull request.

## Documentation

For more information on developing Claude Code plugins, see the [official documentation](https://docs.anthropic.com/en/docs/claude-code).

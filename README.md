# Purexua's Claude Code Plugins

English | [简体中文](README.zh-CN.md)

A curated directory of high-quality plugins for Claude Code by Purexua.

> **⚠️ Important:** Make sure you trust a plugin before installing, updating, or using it. Anthropic does not control what MCP servers, files, or other software are included in plugins and cannot verify that they will work as intended or that they won't change. See each plugin's homepage for more information.

## Structure

- **`/plugins`** - Internal plugins developed and maintained by Purexua
- **`/external_plugins`** - Third-party plugins from partners and the community

## Installation

### Adding the Marketplace

First, add this marketplace using the `/plugin marketplace add` command (shortcut: `/plugin market add`):

```bash
/plugin marketplace add purexua/claude-plugins
```

### Installing Plugins

Once the marketplace is added, install plugins via:

```bash
/plugin install {plugin-name}@purexua-claude-plugins
```

or browse for plugins in `/plugin > Discover`

## Contributing

### Internal Plugins

Internal plugins are developed by Purexua. See `/plugins/example-plugin` for a reference implementation.

### External Plugins

Third-party partners can submit plugins for inclusion in the marketplace. External plugins must meet quality and security standards for approval.

## Plugin Structure

Each plugin follows a standard structure:

```
plugin-name/
├── .claude-plugin/
│   └── plugin.json      # Plugin metadata (required)
├── .mcp.json            # MCP server configuration (optional)
├── .lsp.json            # LSP server configuration (optional)
├── commands/            # Slash commands (optional)
├── agents/              # Agent definitions (optional)
├── skills/              # Skill definitions (optional)
└── README.md            # Documentation
```

## Documentation

For more information on developing Claude Code plugins, see the [official documentation](https://code.claude.com/docs/en/plugins).

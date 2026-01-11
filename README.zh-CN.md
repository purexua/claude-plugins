# Purexua 的 Claude Code 插件

<p align="center">
<a href="README.md">English</a> | 简体中文
</p>

Purexua 精选的高质量 Claude Code 插件目录。

> **⚠️ 重要提示：** 在安装、更新或使用插件之前，请确保您信任该插件。Anthropic 不控制插件中包含的 MCP 服务器、文件或其他软件，也无法验证它们是否按预期工作或是否会发生变化。有关更多信息，请参阅每个插件的主页。

## 结构

- **`/plugins`** - Purexua 开发和维护的内部插件
- **`/external_plugins`** - 来自合作伙伴和社区的第三方插件

## 安装

### 添加市场

首先，使用 `/plugin marketplace add` 命令（快捷方式：`/plugin market add`）添加此市场：

```bash
/plugin marketplace add purexua/claude-plugins
```

### 安装插件

添加市场后，可通过以下方式安装插件：

```bash
/plugin install {plugin-name}@purexua-claude-plugins
```

或在 `/plugin > Discover` 中浏览插件

## 贡献

### 内部插件

内部插件由 Purexua 开发。参考实现请参见 `/plugins/example-plugin`。

### 外部插件

第三方合作伙伴可以提交插件以包含在市场中。外部插件必须符合质量和安全标准才能获得批准。

## 插件结构

每个插件遵循标准结构：

```
plugin-name/
├── .claude-plugin/
│   └── plugin.json      # 插件元数据（必需）
├── .mcp.json            # MCP 服务器配置（可选）
├── .lsp.json            # LSP 服务器配置（可选）
├── commands/            # 斜杠命令（可选）
├── agents/              # 代理定义（可选）
├── skills/              # 技能定义（可选）
└── README.md            # 文档
```

## 文档

有关开发 Claude Code 插件的更多信息，请参阅[官方文档](https://code.claude.com/docs/en/plugins)。

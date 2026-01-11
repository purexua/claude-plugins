# Changelog

All notable changes to this project will be documented in this file.

## [1.0.1] - 2026-01-11

### Fixed
- Fixed incorrect source path in marketplace.json for example-plugin (was pointing to non-existent `./plugins/hello`, now correctly points to `./plugins/example-plugin`)

## [1.0.0] - 2026-01-11

### Added
- Initial release of Purexua's Claude Code Plugin Marketplace
- Comprehensive marketplace documentation with bilingual support (English and Chinese)
- Plugin marketplace configuration (`.claude-plugin/marketplace.json`)
- Directory structure for internal plugins (`/plugins`) and external plugins (`/external_plugins`)
- Installation guide with marketplace setup instructions
- Plugin structure and contribution guidelines
- **code-simplifier** plugin: Simplifies and refines code for clarity, consistency, and maintainability
- **example-plugin**: Reference implementation for plugin developers with example commands and skills
- MIT License
- `.gitignore` for macOS system files

### Documentation
- Complete README.md with marketplace overview, installation, and contribution guidelines
- Chinese translation (README.zh-CN.md) for broader accessibility
- Plugin development documentation and structure reference

[1.0.1]: https://github.com/purexua/claude-plugins/releases/tag/v1.0.1
[1.0.0]: https://github.com/purexua/claude-plugins/releases/tag/v1.0.0

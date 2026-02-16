# Project Structure

## Root Files

- `power.json` - Power manifest with metadata, keywords, and MCP server configuration
- `POWER.md` - Comprehensive user documentation with workflows and troubleshooting
- `README.md` - Quick start guide for installation and setup
- `.gitignore` - Excludes `.kiro/settings/` (contains sensitive MCP configuration)

## Kiro Configuration Directory

`.kiro/` - Kiro-specific configuration (not committed to git)
- `.kiro/settings/` - Sensitive configuration files (gitignored)
- `.kiro/hooks/` - Agent hooks
- `.kiro/steering/` - Steering documents for AI assistant guidance

## File Conventions

### power.json
- Contains name, displayName, version, description
- Keywords array for discoverability
- MCP server configuration under `mcp` key
- Uses environment variable placeholders (e.g., `${TRELLO_API_KEY}`)

### POWER.md
- Primary user documentation
- Sections: Overview, Features, Quick Start, Common Workflows, Authentication, Troubleshooting, Security, Resources
- Includes code examples and configuration snippets
- Natural language workflow examples for users to ask Kiro

### README.md
- Installation instructions (Kiro UI and manual)
- Configuration steps
- Brief usage overview
- Links to detailed documentation in POWER.md

## Security Considerations

- API keys stored in MCP configuration (not in power files)
- Authentication tokens stored in user home directory (`~/.trello_mcp_token.json`)
- Sensitive configuration excluded from version control via `.gitignore`

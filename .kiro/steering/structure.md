# Project Structure

## Root Files

- `POWER.md` - Comprehensive user documentation with frontmatter metadata (name, description, keywords)
- `README.md` - Quick start guide for installation and setup
- `mcp.json` - MCP server configuration
- `.gitignore` - Excludes `.kiro/settings/` (contains sensitive MCP configuration)

## Kiro Configuration Directory

`.kiro/` - Kiro-specific configuration (not committed to git)
- `.kiro/settings/` - Sensitive configuration files (gitignored)
- `.kiro/hooks/` - Agent hooks
- `.kiro/steering/` - Steering documents for AI assistant guidance

## File Conventions

### POWER.md
- Contains frontmatter with name, description, author, and keywords
- Frontmatter uses YAML format between `---` delimiters
- Primary user documentation
- Sections: Overview, Features, Quick Start, Common Workflows, Authentication, Troubleshooting, Security, Resources
- Includes code examples and configuration snippets
- Natural language workflow examples for users to ask Kiro

### mcp.json
- MCP server configuration
- Uses environment variable placeholders (e.g., `${TRELLO_API_KEY}`)

### README.md
- Installation instructions (Kiro UI and manual)
- Configuration steps
- Brief usage overview
- Links to detailed documentation in POWER.md

## Security Considerations

- API keys stored in MCP configuration (not in power files)
- Authentication tokens stored in user home directory (`~/.trello_mcp_token.json`)
- Sensitive configuration excluded from version control via `.gitignore`

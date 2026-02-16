# Technology Stack

## Power Type

Kiro Power - MCP (Model Context Protocol) server integration

## Runtime Requirements

- `uv` package manager (required for uvx command)
- `uvx` command runner (automatically available with uv)
- Trello MCP server package: `trello-mcp-server`

## Configuration Files

- `power.json` - Power metadata, MCP server configuration
- `POWER.md` - User-facing documentation
- `README.md` - Installation and setup guide

## MCP Server Configuration

The power uses the following MCP server setup:
```json
{
  "command": "uvx",
  "args": ["trello-mcp-server"],
  "env": {
    "TRELLO_API_KEY": "${TRELLO_API_KEY}"
  }
}
```

## External Dependencies

- Trello API (REST API via OAuth 1.0a)
- Upstream MCP server: https://github.com/cargom98/gm-trello-mcp

## Common Commands

No build or test commands - this is a configuration-based power that wraps an external MCP server. The MCP server is automatically downloaded and run by uvx when needed.

## Installation

Manual installation:
```bash
git clone https://github.com/cargom98/gm-trello-mcp ~/.kiro/powers/trello
```

Or install via Kiro's Powers UI (Command Palette → "Powers: Configure").

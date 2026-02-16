# Trello Power for Kiro

A Kiro Power that integrates the Trello MCP server, enabling you to manage Trello boards, lists, cards, and organizations directly from your development environment.

## Installation

### Option 1: Install from Kiro (Recommended)

1. Open Kiro
2. Open the Command Palette (Cmd/Ctrl + Shift + P)
3. Search for "Powers: Configure"
4. Search for "Trello" and click Install

### Option 2: Manual Installation

1. Clone this repository to your Kiro powers directory:
   ```bash
   git clone https://github.com/cargom98/gm-trello-mcp ~/.kiro/powers/trello
   ```

2. Ensure `uv` is installed (required for uvx):
   ```bash
   # See https://docs.astral.sh/uv/getting-started/installation/
   ```

3. Restart Kiro

## Configuration

1. Get your Trello API key from [Trello Power-Ups Admin](https://trello.com/power-ups/admin/new)

2. Configure the MCP server in Kiro:
   - Open Command Palette → "MCP: Open Configuration"
   - Add your API key to the `trello` configuration

3. On first use, authorize the application in your browser

## Usage

Once installed and configured, you can ask Kiro to:

- List your Trello boards
- Create and manage lists
- Create, update, and move cards
- Manage organizations and teams

See [POWER.md](POWER.md) for detailed workflows and examples.

## Requirements

- `uv` package manager (for uvx command)
- Trello account
- Trello API key

## Files

- `power.json` - Power configuration and metadata
- `POWER.md` - Complete documentation and workflows
- `README.md` - This file

## Support

For issues or questions, visit the [GitHub repository](https://github.com/cargom98/gm-trello-mcp).

## License

See the [upstream repository](https://github.com/cargom98/gm-trello-mcp) for license details.

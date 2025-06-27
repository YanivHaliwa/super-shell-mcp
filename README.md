# Super Shell MCP Server - Fork with Local Whitelist Persistence

**Original repository:** [https://github.com/cfdude/super-shell-mcp](https://github.com/cfdude/super-shell-mcp)

## What's Different in This Fork

The original Super Shell MCP Server saves all whitelist configurations in memory, which means all whitelist changes are lost whenever the MCP server is restarted.

**This fork saves the whitelist locally to a JSON file:**

- Whitelist persists across MCP server restarts
- Automatically saves to: `~/.config/super-shell-mcp/whitelist.json`
- All original functionality remains unchanged

## Installation

```bash
# Clone this forked repository
git clone https://github.com/YanivHaliwa/super-shell-mcp.git
cd super-shell-mcp

# Install dependencies
npm install

# Build the project
npm run build
```

## Whitelist Configuration Location

The whitelist JSON file is automatically created and managed at:

- **Linux/macOS**: `~/.config/super-shell-mcp/whitelist.json`
- **Windows**: `%APPDATA%\super-shell-mcp\whitelist.json`

Make sure this directory exists and has proper write permissions for the MCP server.

## Author

Created by [Yaniv Haliwa](https://github.com/YanivHaliwa) for enhanced MCP whitelist persistence.

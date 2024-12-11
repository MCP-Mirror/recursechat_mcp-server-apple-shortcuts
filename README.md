# Apple Shortcuts MCP Server 🤖

A Model Context Protocol (MCP) server that lets AI assistants like Claude control Apple Shortcuts automations. This enables AI models to trigger shortcuts and automate tasks on macOS in a safe and controlled way.

## What is MCP? 🤔

The Model Context Protocol (MCP) is a system that lets AI apps, like Claude Desktop, connect to external tools and data sources. It gives a clear and safe way for AI assistants to work with local services and APIs while keeping the user in control.

## What does this server do? 🚀

The Apple Shortcuts MCP server:
- Enables AI assistants to list available shortcuts
- Allows running shortcuts by name with optional input parameters 
- Provides a simple interface for automation control

## Prerequisites 📋

Before you begin, ensure you have:

- [Node.js](https://nodejs.org/) (v18 or higher)
- [Claude Desktop](https://claude.ai/download) installed
- macOS with Shortcuts app configured

## Configuration to use Apple Shortcuts Server
Here's the Claude Desktop configuration to use the Apple Shortcuts server:

```json
{
  "mcpServers": {
    "apple-shortcuts": {
      "command": "npx",
      "args": ["-y", "mcp-server-apple-shortcuts"]
    }
  }
}
```

## Usage

You can ask Claude "list shortcuts" or run a specific shortcut with the shortcut name, for example "get word of the day" or "play a song".

## License

Apache-2.0
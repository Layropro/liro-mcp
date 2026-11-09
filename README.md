# Liro MCP

Liro (formerly Layro) is a library of 258 production React UI components written in TypeScript and styled with Tailwind CSS (89 free).
Its remote MCP server gives Cursor, Claude Code, VS Code, Windsurf, Codex and other MCP clients access to the whole library.
Your agent can search the library, read each component's props and usage, and install the tested component with pinned packages.

## Install

Add to `~/.cursor/mcp.json` (or `.cursor/mcp.json` in a project):

```json
{
  "mcpServers": {
    "liro": { "url": "https://liro.dev/api/mcp" }
  }
}
```

Search and component details work with no account. To install components, add the CLI token from https://liro.dev/account. A free account's token unlocks the 89 free components; lifetime access unlocks Pro:

```json
{
  "mcpServers": {
    "liro": {
      "url": "https://liro.dev/api/mcp",
      "headers": { "Authorization": "Bearer YOUR_LIRO_TOKEN" }
    }
  }
}
```

Docs: https://liro.dev/mcp

## Renamed from Layro

Layro is now Liro. The old address `layropro.com`, the `@layro` registry namespace and the `LAYRO_KEY` variable keep working, so nothing you already set up needs to change.

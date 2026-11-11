# Installing the Aworkado MCP server

Aworkado is a remote MCP server. There is nothing to clone, build or run locally, and no API key.

Add this entry to the client's MCP settings (for Cline: `cline_mcp_settings.json`):

```json
{
  "mcpServers": {
    "aworkado": {
      "type": "streamableHttp",
      "url": "https://aworkado.co/mcp"
    }
  }
}
```

Check the connection by calling `search_jobs` with `{"jobFunction": "Software Engineering", "region": "europe"}`. It should return up to ten job postings, each with an aworkado.co link.

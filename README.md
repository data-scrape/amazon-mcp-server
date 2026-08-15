<div align="center">

# Amazon Mcp Server

**MCP server for Amazon public-data workflows** — expose focused tools to compatible AI clients.

![MCP](https://img.shields.io/badge/MCP-Compatible-7C3AED?style=flat)
![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=flat)

</div>

## Agent job: product research and price-monitoring workflows

This server gives an MCP-compatible client a narrow tool surface for Amazon tasks. The design principle is: request a specific question, return structured records with source context, then let the agent explain or act with those records.

## Quick configuration

```json
{
  "mcpServers": {
    "amazon": {
      "command": "uvx",
      "args": ["amazon-mcp-server"]
    }
  }
}
```

## Example tool call

```text
amazon_search(query="wireless headphones", limit=10)
```

Use a small result limit first. In a production agent, validate arguments, preserve source metadata, restrict sensitive actions, and log tool outcomes.


## License

MIT License.

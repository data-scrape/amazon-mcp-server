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

<!-- CROSS_LINKS_START -->

## Related projects

Explore these closely related implementation paths:

- [amazon-product-api](https://github.com/data-scrape/amazon-product-api) — Amazon Product API - Real-time product, pricing, and review data via REST API
- [best-amazon-scraper](https://github.com/data-scrape/best-amazon-scraper) — Best Amazon Scraper - Extract product data, prices, reviews, and BSR via API
- [google-maps-mcp-server](https://github.com/data-scrape/google-maps-mcp-server) — Google Maps MCP Server - AI agent access to local business data via MCP
- [linkedin-mcp-server](https://github.com/data-scrape/linkedin-mcp-server) — LinkedIn MCP Server - Give AI agents access to profiles, companies, and jobs via Model Context Protocol
- [best-google-maps-scraper](https://github.com/data-scrape/best-google-maps-scraper) — Best Google Maps Scraper - Extract business data, reviews, ratings & contact info via API
- [best-instagram-scraper](https://github.com/data-scrape/best-instagram-scraper) — Best Instagram Scraper - Extract posts, profiles, stories, and hashtag data via API

<!-- CROSS_LINKS_END -->
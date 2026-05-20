# XiaoHongShu Search Skill

Install this agent skill to search XiaoHongShu / RED / RedNote through the hosted whatson.red MCP endpoint and receive structured JSON results.

## Install

```bash
npx skills add seichris/xiaohongshu-search-mcp-skill --skill xiaohongshu-search
```

## Requirements

Create an Agent API key at https://www.whatson.red/agents and set:

```bash
export WHATSON_RED_API_KEY="your_api_key"
```

The skill uses:

- MCP endpoint: `https://www.whatson.red/api/agent/mcp`
- MCP tool: `search_xiaohongshu_notes`
- Auth header: `Authorization: Bearer ${WHATSON_RED_API_KEY}`

MCP requests use whatson.red account credits. x402 payment is available only through the REST API, not MCP.

## Skill

The installable skill lives at:

```text
skills/xiaohongshu-search/SKILL.md
```

This repository intentionally contains only the public skill package. It does not include Browserless configuration, cookies, proxies, backend code, or deployment secrets.

# Airport Taxi Hub assistant plugins

Listing packages that put [Airport Taxi Hub](https://airporttaxihub.com) fixed-price airport transfers into AI assistants.
Each folder is one host's package. They hold manifests, a skill, listing text and images only; every package points at the same
public MCP server run by Airport Taxi Hub, and no server code lives here.

| Folder | Host | Server URL |
|---|---|---|
| `claude/` | Claude (chat, Cowork, Claude Code) | `https://mcp.airporttaxihub.com/mcp/claude` |
| `chatgpt/` | ChatGPT (OpenAI plugin package) | `https://mcp.airporttaxihub.com/mcp` |

Booking always finishes on airporttaxihub.com; no payment or personal details pass through these packages.

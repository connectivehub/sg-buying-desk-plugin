# Singapore Buying Desk: plugin for Cursor and other agents

Singapore Buying Desk helps office managers and small teams in Singapore buy office, IT and event-print supplies. It gives firm, GST-inclusive SGD quotes with delivery dates from a trade catalog that is refreshed daily, so a whole list can be priced and ordered in one chat instead of calling vendors.

This repository holds only the plugin package: the manifest, the MCP configuration and one skill. The server is hosted by Connective Labs Pte. Ltd. (UEN 202543350R).

## What it does

- Prices office and IT supplies (cables, storage, peripherals, monitors, UPS units, networking, ink and toner), with 9% GST and Singapore delivery included.
- Prices event print (name cards, lanyards, roll-up banners, tote bags).
- Prices a list of items in one call and turns it into a firm quote request.
- Looks up Singapore addresses, public holidays, working days, weather, PSI and everyday errands.

No payment is taken in chat. A buyer approves a firm quote and pays Connective Labs by PayNow or a payment link. Delivery is within Singapore only.

## Install

Install it from the Cursor Marketplace, or add the server to any MCP client yourself:

```json
{"mcpServers": {"sg-buying-desk": {"url": "https://mcp.connective-labs.com/sg-buying-desk/mcp"}}}
```

The server uses Streamable HTTP and needs no sign-in or API key.

## Try it

- "Price two 5m HDMI cables delivered in Singapore by Friday"
- "Quote 3 HP 206A cyan toners for our office"
- "Quote 200 lanyards for an event next month"

## Contents

- `plugin.json`: Agent Plugins manifest
- `.cursor-plugin/plugin.json`: Cursor plugin manifest
- `mcp.json`: MCP server configuration
- `skills/buy-supplies-singapore/SKILL.md`: how an agent should use the tools
- `assets/`: logo and icon

## Links

- Website: https://mcp.connective-labs.com/
- Support: https://mcp.connective-labs.com/support
- Privacy: https://mcp.connective-labs.com/privacy
- Terms: https://mcp.connective-labs.com/terms

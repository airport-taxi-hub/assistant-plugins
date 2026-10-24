# Airport Taxi Hub for Claude

Live, fixed prices for private airport and hotel transfers inside Claude. Ask for a transfer between an airport and a hotel,
address or city centre, one-way or return, and Claude shows the vehicles that fit your party and luggage with their total prices.
You finish the booking on [airporttaxihub.com](https://airporttaxihub.com), where the flight number, exact address, names and
payment are added. Prices in Claude are the same as on the website.

## Install

In Claude, add it from the plugin directory. In Claude Code:

```
/plugin install airport-taxi-hub --marketplace airport-taxi-hub/assistant-plugins
```

## What this plugin contains

- **Connector:** one remote MCP server, `https://mcp.airporttaxihub.com/mcp/claude`, run by Airport Taxi Hub. No sign-in.
  It exposes one read-only tool, `search_transfers`, and one card that shows the results.
- **Skill:** `airport-transfer-quotes`, which tells Claude which trip details a quote needs and how to read the results.

## What is sent, and where

When Claude asks for a quote, it sends the pickup and drop-off place names (or the place ids from an earlier result), the pickup
date and time, the number of passengers and suitcases, an optional return date and time, and the language of the conversation to
`mcp.airporttaxihub.com`. Nothing else: no names, email addresses, phone numbers, flight numbers or payment details are asked for
or sent. The server looks up places and routes with Google Maps and prices the journey; a short-lived quote record (30 minutes) is
kept so the Book link can open the same prices. The plugin runs no local code and contacts no other service.

## Example prompts

- "Taxi from Edinburgh Airport to The Balmoral hotel in Edinburgh next Saturday at 9:30am, 2 of us with 2 suitcases. How much?"
- "Return transfer from Heathrow to The Savoy, landing Friday at 08:00 and back Monday at 18:00, 2 people, 2 suitcases."
- "Cheapest way for 8 of us with 8 bags from Stansted Airport to Cambridge next month at noon."

## Support and policies

- Help: https://airporttaxihub.com/help#contact-us
- Privacy policy: https://airporttaxihub.com/privacy-policy
- Terms of service: https://airporttaxihub.com/terms-of-service

## Privacy Policy

Airport Taxi Hub's privacy policy, at https://airporttaxihub.com/privacy-policy, covers data collection, use and storage,
third-party sharing, retention and contact details. Through this plugin, only the journey details listed above are processed.

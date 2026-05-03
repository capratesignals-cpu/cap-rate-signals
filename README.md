# Cap Rate Signals — US Real Estate Investment Intelligence

An MCP server that identifies US real estate markets repricing ahead of consensus — before workers arrive and housing prices move.

## What it does

Tracks confirmed corporate investment (semiconductor fabs, pharma plants, defense campuses, data centers, military installations) across 40+ US metros and scores them based on worker arrival timing, cap rate trajectory, and entry price. The window to buy is before demand arrives, not after.

## Tools (14 total)

| Tool | Description |
|---|---|
| `get_top_picks` | Top NOW and NEXT markets ranked by conviction |
| `get_metro_brief` | Full investment brief on a specific city |
| `find_metros` | Discover markets by region, theme, employer, or budget |
| `assess_metro` | Raw data record — score, cap rate, vacancy, entry price |
| `compare_metros` | Head-to-head comparison of two markets |
| `get_tier` | All markets at a given investment tier (NOW/NEXT/LATER) |
| `get_alerts` | Signal feed — what moved this week |
| `get_regional_comps` | Best comparable markets in the same region |
| `get_metro_map_data` | Annotated map with employer pins and target zip codes |
| `get_weekly_review` | Admin: stale flags and pending tier proposals |
| `set_published_tier` | Admin: update published tier for a metro |
| `clear_stale_progress_flag` | Admin: clear stale progress flag |
| `ping` | Server version check |
| `log_missed_query` | Log queries that fell through tool routing |

## Example queries

- *"Where should I invest right now?"*
- *"Is Indianapolis a good market?"*
- *"Show me semiconductor markets under $300K"*
- *"What moved this week?"*
- *"Compare Sherman TX and Tulsa"*
- *"Show me defense markets in the southeast"*

## Connect

```bash
smithery mcp add capratesignals/cap-rate-signals
```

Or use the MCP server URL directly:
```
https://cap-rate-signals-mcp-production.up.railway.app/mcp
```

No authentication required. Transport: Streamable HTTP.

## Coverage

Markets tracked: Sherman TX, Indianapolis IN, Columbus OH, West Lafayette IN, Knoxville TN, Tulsa OK, Boise ID, Lehigh Valley PA, St. Louis MO, Clayton NC, Wilmington DE, and more across the US.

Catalyst types: Semiconductor (CHIPS Act), Pharma/Biotech, Defense/Military, Data Centers, EV/Automotive, Logistics, College Towns, Nuclear Energy, Aerospace.

---

Powered by [Cap Rate Signals](https://capratesignals.com)

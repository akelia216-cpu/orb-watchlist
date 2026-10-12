# orb-watchlist

One file, `watchlist.json`, written each weekday morning before 9:30 ET. A paper-trading bot reads it and watches those stocks for an opening range breakout. Paper only, no real money. Not advice.

Format:

```json
{"date": "2026-10-13", "symbols": [{"symbol": "ABC", "why": "one line on the news"}]}
```

The bot ignores the file unless `date` is today (US Eastern), takes at most 5 symbols, and only stocks priced between $5 and $200.

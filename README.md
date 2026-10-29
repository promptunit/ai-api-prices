# AI API prices, every day

Per-token prices for OpenAI, Anthropic (Claude), Google (Gemini) and xAI (Grok) models, read once a day from each vendor's own pricing page.

- `prices.json`: today's list
- `history/YYYY-MM-DD.json`: one file per day, so you can see when a price changed

All prices are in USD per 1 million tokens. Each model has `input`, `output`, `cachedInput` and `cacheWrite` prices, a higher `longPrompt` price where the vendor charges one, the context window, the release date, and a link to its page on promptunit.ai.

A vendor whose page could not be read that day is listed under `vendorsNotRead`. Its models are left out rather than filled in with old numbers.

## Use it

```sh
curl -s https://raw.githubusercontent.com/promptunit/ai-api-prices/main/prices.json
```

Or straight from the source: https://www.promptunit.ai/ai-api-pricing/prices.json

The same list, with a page per model and side-by-side comparisons: https://www.promptunit.ai/ai-api-pricing

## License

CC BY 4.0. Use it anywhere, credit "PromptUnit" with a link to https://www.promptunit.ai/ai-api-pricing.

Spotted a wrong price? Open an issue with a link to the vendor's page.

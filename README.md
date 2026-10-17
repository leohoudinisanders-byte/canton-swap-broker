# Canton Swap Broker

Pay-per-call swap access to the Canton Network via the [OneSwap](https://oneswap.cc) atomic DvP DEX. AI agents pay per request in USDC on Base through x402 v2 — no API keys, no subscription.

- **Landing + docs:** https://leohoudinisanders-byte.github.io/canton-swap-broker/
- **Live endpoint:** https://solene-fa2010da.base44.app/functions/cantonSwapBroker?action=info
- **OpenAPI spec:** [openapi.json](openapi.json) (OpenAPI 3.1)
- **Marketplace:** Listed and payment-verified on [PayAPI Market](https://payapi.market/api/canton-swap-broker)

## Endpoints

| Action | Price | Returns |
|---|---|---|
| `quote` | $0.02 | Settlement-accurate pool quote (fees, impact, network fee included) |
| `createSwap` | $0.05 | Escrow swap: depositParty, minOut, 1-hour deadline |
| `markets` | $0.02 | All Canton pools, reserves, fees, optional tickers |
| `tokens` | $0.02 | Settleable token registry with issuer Party IDs |
| `cancel` | $0.02 | Cancel a pre-deposit escrow swap |
| `status` / `openSwap` | free | Swap lifecycle reads |
| `info` | free | Machine-readable directory |

## Related service

[On-chain Forensics API](https://leohoudinisanders-byte.github.io/onchain-forensics/) — pay-per-call token verdicts, supply audits, and wallet-flow analysis on Base and Ethereum, same x402 pay-per-call model.

---
Contact: Leo Sanders · Payments: USDC on Base via x402 v2 ([x402.org](https://x402.org)) · Swaps powered by [OneSwap](https://oneswap.cc) on Canton

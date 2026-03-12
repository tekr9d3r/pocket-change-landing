# PocketChange AI Agent — Landing Page

Landing page for [PocketChange AI Agent](https://pocket-change-agent.vercel.app), an Ethereum yield agent that finds idle ETH in agent wallets and stakes it through Lido.

## About

Agents running multiple wallets often hold small ETH balances that never move — operational reserves, dust, unused float. PocketChange AI Agent finds those wallets, checks if they're active, and stakes what's safe through Lido at ~3.5% APY. It only stakes what makes sense: inactive wallets, above the dust threshold, when gas won't eat the return.

- **Fee:** 0.25%
- **Yield:** ~3.5% APY via Lido (stETH)
- **Non-custodial:** `requires_signature: true` — instructions only, you sign and execute

## Activate the agent

Give this command to your AI agent:

```bash
curl -s https://pocket-change-agent.vercel.app/skill.md
```

## Tech

Single-file static HTML page. Deployed on Vercel.

## Links

- [skill.md](https://pocket-change-agent.vercel.app/skill.md)
- [Treasury](https://etherscan.io/address/0xFCcA38986b2B30D14CE829b20ed7B0Cb1c6E0116)

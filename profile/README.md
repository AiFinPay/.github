<div align="center">

# AiFinPay

<img src="../assets/20260430-020219.jpg" width="120" height="120" alt="AiFinPay logo" />

### The payment protocol for autonomous AI agents

Stripe for AI agents — non-custodial, pay-per-call, on-chain settlement.

[Website](https://aifinpay.io) · [Docs](https://docs.aifinpay.io) · [Integration Guide](https://github.com/AiFinPay/aifinpay-agent-integration)

</div>

---

## What is AiFinPay?

AiFinPay gives any AI agent a wallet so it can pay — and get paid — for services on-chain. Built on the open **x402** protocol and the **AIFP** standards, it enables autonomous machine-to-machine commerce with per-call settlement across multiple blockchains.

- **Pay-per-call** — agents settle each invocation exactly, no subscriptions, no pre-funding.
- **Non-custodial** — payments flow directly wallet-to-wallet; no intermediary holds funds.
- **Multi-chain** — EVM, Solana, Aptos and more (and growing).
- **Agent-first** — MCP server + SDK so any agent framework can plug in minutes.

## Protocol & Standards

| Repo                                         | Description |
|----------------------------------------------|---|
| [AIFP_1](https://github.com/AiFinPay/AIFP-1) | Open protocol for AI-native payments, paywalls, agent identity, and autonomous M2M commerce. |
| [AIFP_2](https://github.com/AiFinPay/AIFP-2) | Core agent payment protocol — routing, wallet policy, settlement verification and receipts; x402 v2 compatibility profile. |
| [AIFP_3](https://github.com/AiFinPay/AIFP-3) | Global Agent Passport — immutable identity, issuer/holder keys, lifecycle, and verified wallet bindings. |
| [AIFP_4](https://github.com/AiFinPay/AIFP-4) | Open organization / corporation protocol. |
| [AIFP_5](https://github.com/AiFinPay/AIFP-5-Quantum-Safe-Financial-Protocol) | Quantum-safe authorization envelopes — classical, hybrid, and post-quantum cryptographic authorization. |
| [AIFP_6](https://github.com/AiFinPay/AIFP-6-Agentic-Financial-Governance-Protocol) | Agentic financial governance — machine-readable authority, limits, delegation, approvals, emergency controls and audit decisions. |

## On-Chain Contracts

| Repo | Chain | Language | Highlights |
|---|---|---|---|
| [evm-contract](https://github.com/AiFinPay/evm-contract) | Polygon | Solidity | `AiFinPayCore v1.1` with Pyth Pull Oracle. |
| [aifinpay-avalanche](https://github.com/AiFinPay/aifinpay-avalanche) | Avalanche C-Chain | Solidity | Live & verified on mainnet (43114). Per-call settlement via Pyth + on-chain splitter. |
| [solana-contract](https://github.com/AiFinPay/solana-contract) | Solana | Rust | Anchor program — Seat PDAs, `b2b_pay`, `b2b_pay_with_split`. Live on mainnet. |

## Tools & Integrations

| Repo | Description |
|---|---|
| [sdk](https://github.com/AiFinPay/sdk) | TypeScript SDK for embedding AiFinPay into agents and services. |
| [aifinpay-cli](https://github.com/AiFinPay/aifinpay-cli) | Agent-first CLI (Go). Pay-per-call x402 + on-chain settlement; wraps `@aifinpay/mcp`. |
| [aifinpay-agent-integration](https://github.com/AiFinPay/aifinpay-agent-integration) | Official integration guide — give any AI agent a wallet (MCP + SDK). |
| [stellar-x402-facilitator](https://github.com/AiFinPay/stellar-x402-facilitator) | Open-source x402 facilitator & Bazaar discovery layer for Stellar. |

## Documentation

- [docs](https://github.com/AiFinPay/docs) — AiFinPay developer documentation (Mintlify).

## Supported Chains

Settlement contracts deployed across **14 mainnet networks**:

EVM compatible
<table>
  <tr>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/arc.svg" width="32" alt="Avalanche" /><br>Arc</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/avalanche.svg" width="32" alt="Avalanche" /><br>Avalanche</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/arbitrum.png" width="32" alt="Arbitrum" /><br>Arbitrum</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/polygon.svg" width="32" alt="Polygon" /><br>Polygon</a></td>
  </tr> 
  <tr>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/bnb.svg" width="32" alt="BNB Chain" /><br>BNB Chain</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/base.svg" width="32" alt="Base" /><br>Base</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/robinhood.png" width="32" alt="Robinhood" /><br>Robinhood</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/optimism.svg" width="32" alt="Optimism" /><br>Optimism</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/xrpl.svg" width="32" alt="XRPL EVM" /><br>XRPL EVM</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/unichain.svg" width="32" alt="Unichain" /><br>Unichain</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/evm-contract"><img src="../assets/chains/botchain.svg" width="32" alt="BOT Chain" /><br>BOT Chain</a></td>
  </tr>
</table>

Non EVM
<table>
  <tr>
    <td align="center"><a href="https://github.com/AiFinPay/solana-contract"><img src="../assets/chains/solana.svg" width="32" alt="Solana" /><br>Solana</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/near-contract"><img src="../assets/chains/near.svg" width="32" alt="NEAR" /><br>NEAR</a></td>
    <td align="center"><a href="https://github.com/AiFinPay/aptos-contract"><img src="../assets/chains/aptos.svg" width="32" alt="Aptos" /><br>Aptos</a></td>
  </tr>
</table>

Live state varies per chain — see the
[network source-of-truth](https://github.com/AiFinPay/knowledge-vault/blob/main/docs/10-projects/aifinpay/network-source-of-truth.md)
for the per-layer status matrix.

## Getting Started

Install the package(s) you need and give your agent a funded wallet:

```bash
# MCP server — plug any agent framework into AiFinPay
npm install @aifinpay/mcp

# Opinionated agent runtime (optional)
npm install @aifinpay/agents

# Or scaffold a full integration
npx @aifinpay/cli init
```

Then point your agent at the MCP server and give it a funded wallet. See the
[integration guide](https://github.com/AiFinPay/aifinpay-agent-integration) for details.

<div align="center">

---

Building the rails for autonomous machine-to-machine commerce.

</div>
<div align="center">

<!-- Animated Header -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1956FC,100:00D4FF&height=200&section=header&text=EdgePoly&fontSize=80&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Chain-Reaction%20Automation%20for%20Prediction%20Markets&descAlignY=55&descSize=18" width="100%" />

<!-- Animated Logo -->
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=28&duration=3000&pause=1000&color=1956FC&center=true&vCenter=true&multiline=true&repeat=false&width=600&height=100&lines=Automate.+Execute.+Win." alt="Tagline" />

<br />

<!-- Badges -->
[![Website](https://img.shields.io/badge/Website-edgepoly.fun-1956FC?style=for-the-badge&logo=googlechrome&logoColor=white)](https://edgepoly.fun)
[![Documentation](https://img.shields.io/badge/Docs-Read%20Now-00D4FF?style=for-the-badge&logo=readthedocs&logoColor=white)](https://docs.edgepoly.fun)
[![Twitter](https://img.shields.io/badge/Twitter-Follow%20Us-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/edgepolyfun)

<br />

<!-- Stats Animation -->
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=16&duration=2000&pause=500&color=00D4FF&center=true&vCenter=true&width=800&lines=%24127M%2B+Volume+Automated;15K%2B+Active+Chains;99.7%25+Uptime;%3C50ms+Execution+Latency" alt="Stats" />

</div>

---

## What is EdgePoly?

**EdgePoly** is the first chain-reaction automation platform for prediction markets. We enable traders to create sophisticated, interconnected trading strategies that execute automatically based on market conditions, event outcomes, and custom triggers.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   IF Market A resolves YES                                              │
│     └─► THEN Buy Market B at 0.35                                       │
│           └─► IF Market B reaches 0.65                                  │
│                 └─► THEN Take Profit + Notify                           │
│                       └─► THEN Rotate to Market C                       │
│                                                                         │
│   One trigger. Multiple reactions. Exponential edge.                    │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Our Repositories

<table>
<tr>
<td width="50%">

### [@edgepoly/sdk](https://github.com/EdgePolyFun/edgepoly-sdk)

<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" /> <img src="https://img.shields.io/badge/Production-Ready-00C853?style=flat" />

The official TypeScript SDK for building chain-reaction automations.

**Features:**
- Fluent chain builder API
- 6 chain types (link, hedge, split, cascade, conditional, rebalance)
- Advanced conditions engine
- Risk management (Kelly criterion, position sizing)
- Real-time market analytics
- WebSocket support

```typescript
await client
  .chain('My Strategy')
  .whenPriceAbove('market-id', 'yes', 0.7)
  .thenBuy('target-market', 'yes', { amount: 100 })
  .withStopLoss(0.15)
  .deploy();
```

</td>
<td width="50%">

### [@edgepoly/strategies](https://github.com/EdgePolyFun/edgepoly-strategies)

<img src="https://img.shields.io/badge/Trading-Strategies-1956FC?style=flat" /> <img src="https://img.shields.io/badge/Backtesting-Included-FF6B6B?style=flat" />

Production-ready trading strategies collection.

**Strategies:**
- Momentum Trend Follower
- Mean Reversion Contrarian
- Narrative Cascade
- Smart DCA
- Volatility Breakout

**Includes:**
- Full backtesting engine
- 20+ technical indicators
- Signal aggregation system
- Performance analytics

```typescript
const result = await engine.run(strategy, {
  initialCapital: 10000,
  startDate: new Date('2025-12-12'),
});
```

</td>
</tr>
</table>

---

## Chain Types

<table>
<tr>
<td align="center" width="33%">

### Link Order
```
[A] ──► [B]
```
**Sequential execution**

When A triggers, execute B.
Classic if-then automation.

</td>
<td align="center" width="33%">

### Hedge-Link
```
[A] ──┬──► [B]
      └──► [C]
```
**Risk mitigation**

Automatically hedge positions
when conditions change.

</td>
<td align="center" width="33%">

### Split Order
```
      ┌──► [B] 40%
[A] ──┼──► [C] 35%
      └──► [D] 25%
```
**Portfolio distribution**

Distribute capital across
multiple targets.

</td>
</tr>
<tr>
<td align="center" width="33%">

### Cascade
```
[A] ──► [B] ──► [C] ──► [D]
```
**Multi-stage chains**

Execute complex sequences
with multiple stages.

</td>
<td align="center" width="33%">

### Conditional
```
      ┌─ if X ─► [B]
[A] ──┤
      └─ if Y ─► [C]
```
**Dynamic branching**

Choose paths based on
real-time conditions.

</td>
<td align="center" width="33%">

### Rebalance
```
[Portfolio]
    ↓
┌───┴───┐
↓       ↓
[+A]   [-B]
```
**Auto-rebalancing**

Maintain target allocations
automatically.

</td>
</tr>
</table>

---

## Technology Stack

<div align="center">

| Layer | Technologies |
|:---:|:---|
| **Frontend** | ![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-38B2AC?style=flat&logo=tailwind-css&logoColor=white) ![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat&logo=three.js&logoColor=white) |
| **Blockchain** | ![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=flat&logo=ethereum&logoColor=white) ![Polygon](https://img.shields.io/badge/Polygon-8247E5?style=flat&logo=polygon&logoColor=white) ![Viem](https://img.shields.io/badge/Viem-1C1C1C?style=flat) ![Wagmi](https://img.shields.io/badge/Wagmi-1C1C1C?style=flat) |
| **Backend** | ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white) ![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white) |
| **Integrations** | ![Polymarket](https://img.shields.io/badge/Polymarket-000000?style=flat) ![RainbowKit](https://img.shields.io/badge/RainbowKit-7B3FE4?style=flat) |

</div>

---

## Why EdgePoly?

<table>
<tr>
<td width="25%" align="center">

### Never Miss

Traditional trading requires constant attention. EdgePoly watches markets 24/7 and executes the moment your conditions are met.

</td>
<td width="25%" align="center">

### Chain Reactions

Link multiple markets together. When one event triggers, cascade through your entire strategy automatically.

</td>
<td width="25%" align="center">

### Risk Managed

Built-in stop losses, position limits, and hedging. Your capital is protected even when you're away.

</td>
<td width="25%" align="center">

### Battle-Tested

Production-grade strategies backtested across thousands of market scenarios.

</td>
</tr>
</table>

---

## Quick Start

```bash
# Install the SDK
npm install @edgepoly/sdk

# Install strategies (optional)
npm install @edgepoly/strategies
```

```typescript
import { EdgePoly } from '@edgepoly/sdk';

// Initialize
const client = new EdgePoly({
  apiKey: 'your-api-key',
  environment: 'mainnet',
});

// Connect wallet
await client.connect();

// Create your first chain
const chain = await client
  .chain('Election Cascade')
  .type('cascade')
  .source('election-market-id', 'yes')
  .whenResolved('yes')
  .thenBuy('policy-market-id', 'yes', { percentage: 50 })
  .thenNotify('Chain executed!')
  .deploy();

console.log(`Chain deployed: ${chain.id}`);
```

---

## Roadmap

<table>
<tr>
<td width="25%" valign="top">

### Q4 2025
- [x] SDK v1.0 Release
- [x] 5 Core Strategies
- [x] Backtesting Engine
- [x] Multi-wallet Support

</td>
<td width="25%" valign="top">

### Q1 2026
- [ ] Mobile App (iOS/Android)
- [ ] Social Trading
- [ ] Strategy Marketplace
- [ ] Copy Trading

</td>
<td width="25%" valign="top">

### Q2 2026
- [ ] AI Strategy Builder
- [ ] Cross-chain Support
- [ ] Institutional API
- [ ] Advanced Analytics

</td>
<td width="25%" valign="top">

### Q3 2026
- [ ] DAO Governance
- [ ] Protocol Token
- [ ] Decentralized Execution
- [ ] Global Expansion

</td>
</tr>
</table>

---

## Community & Support

<div align="center">

| Channel | Purpose |
|:---:|:---|
| [![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/edgepolyfun) | Announcements, market insights, updates |
| [![Docs](https://img.shields.io/badge/Docs-00D4FF?style=for-the-badge&logo=readthedocs&logoColor=white)](https://docs.edgepoly.fun) | Technical documentation, tutorials, API reference |
| [![Email](https://img.shields.io/badge/Email-1956FC?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hello@edgepoly.fun) | Business inquiries, partnerships |

</div>

---

## Contributing

We love contributions! Whether it's:

- Reporting bugs
- Suggesting new features
- Creating new strategies
- Improving documentation
- Writing tutorials

Check out our [Contributing Guide](https://github.com/EdgePolyFun/edgepoly-sdk/blob/main/CONTRIBUTING.md) to get started.

---

## License

All EdgePoly repositories are released under the [MIT License](LICENSE).

---

<div align="center">

<br />

### Build Your Edge

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=14&duration=4000&pause=1000&color=1956FC&center=true&vCenter=true&width=500&lines=The+future+of+prediction+markets+is+automated.;Start+building+with+EdgePoly+today." alt="CTA" />

<br />

[![Get Started](https://img.shields.io/badge/Get%20Started-edgepoly.fun-1956FC?style=for-the-badge&logo=rocket&logoColor=white)](https://edgepoly.fun)

<br />

---

<sub>Built with dedication by the EdgePoly Team</sub>

<br />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1956FC,100:00D4FF&height=100&section=footer" width="100%" />

</div>

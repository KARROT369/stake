# 🎮 Stake

**Gamified Staking Platform for Karrot**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen)](https://karrot369.github.io/stake/)

---

## Overview

The **Stake** platform is the central gamified staking hub for the Karrot ecosystem. It combines multiple staking modes, XP progression, leaderboards, and achievement systems to create an engaging DeFi experience that rewards both participation and loyalty.

**Live Site:** https://karrot369.github.io/stake/

---

## Features

### 🎰 Multi-Mode Selector
Choose from multiple staking strategies:
- **Standard Stake**: Base APY, flexible withdrawal
- **Locked Stake**: Higher APY with time commitment
- **NFT-Boosted**: Enhanced rewards with NFT ownership
- **Entropy Mode**: Volatility-based variable rewards

### 🏆 Gamification System
- **XP Accumulation**: Earn XP for every staking action
- **Level Progression**: 50+ levels with increasing benefits
- **Leaderboards**: Compete with other stakers
- **Achievements**: Unlock badges and special rewards

### 🎁 Reward Tiers
| Level | XP Required | Reward Multiplier | Special Perk |
|-------|-------------|-------------------|--------------|
| 1 | 0 | 1.0x | - |
| 5 | 1,000 | 1.1x | Early access |
| 10 | 5,000 | 1.25x | Bonus airdrops |
| 25 | 25,000 | 1.5x | Governance rights |
| 50 | 100,000 | 2.0x | VIP status |

---

## Technology Stack

- **Frontend:** React + Vite + Tailwind CSS
- **Smart Contracts:** Solidity 0.8.19+
- **Network:** PulseChain
- **Wallet Support:** MetaMask, WalletConnect

---

## Smart Contracts

### FlippedGamifiedStaking.sol
Main staking contract with gamification features.

**Key Functions:**
- `stake(uint256 amount)` - Stake KARROT tokens
- `unstake(uint256 amount)` - Unstake tokens
- `claimReward()` - Claim RH rewards
- `emergencyWithdraw()` - Emergency exit with penalty
- `getLevel(address user)` - View user's level
- `getXP(address user)` - View user's XP

### RewardDistribution.sol
Manages reward calculations and distributions.

---

## XP System

### Earning XP
| Action | XP Earned |
|--------|-----------|
| Stake | 1 XP per token per second |
| Claim Rewards | 100 XP |
| Level Up | 500 XP bonus |
| 7-Day Streak | 1,000 XP |
| 30-Day Streak | 5,000 XP |

### Level Benefits
- Higher reward multipliers
- Reduced withdrawal penalties
- Exclusive NFT drops
- Governance voting power
- Early access to new features

---

## How It Works

1. **Connect Wallet** to the stake platform
2. **Select Mode** (Standard, Locked, NFT-Boosted, Entropy)
3. **Stake KARROT** tokens
4. **Earn XP** automatically as you stake
5. **Level Up** to unlock multipliers and perks
6. **Compete** on the leaderboard
7. **Claim Rewards** in RH tokens

---

## Emergency Withdraw

In case of emergency, users can withdraw immediately with a **10% penalty**:
- 90% of principal returned
- Forfeited rewards distributed to other stakers
- No time restrictions

---

## Deployment

### Testnet
```bash
npm install
npm run build
npm run deploy:testnet
```

### Mainnet
```bash
npm run build
npm run deploy:mainnet
```

---

## Contract Addresses

| Network | Contract | Address |
|---------|----------|---------|
| PulseChain Testnet | FlippedGamifiedStaking | TBD |
| PulseChain Mainnet | FlippedGamifiedStaking | TBD |

---

## Security

- ✅ ReentrancyGuard on all external functions
- ✅ Emergency withdrawal available
- ✅ XP calculation precision (1e18)
- ✅ Immutable contract design

---

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

---

## License

MIT License - see [LICENSE](LICENSE) file for details.

---

## Connect

- **Website:** https://karrot369.github.io/stake/
- **GitHub:** https://github.com/KARROT369
- **Ecosystem:** KARROT369 DeFi + DadBule VTOL + Nova AI

---

*Built with 🥕 by Peter, Neural Familiar*

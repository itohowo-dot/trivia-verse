
# **trivia-verse – Web3 trivia-verseGame**

trivia-verse is a Web3 trivia-verseGame built on the Base network. Players can play quiz rounds, answer questions, and earn real ETH rewards on-chain.

---

## 📱 **Overview**

trivia-verse is a fun, lightweight Web3 trivia-verseGame designed to showcase:

* **Seamless Web3 wallet integration**
* **Fast L2 transactions on Base**
* **Real ETH rewards**
* **Smooth gameplay experience**
* **Secure, simple blockchain architecture**

Players can:

1. Connect their Web3 wallet (MetaMask, Coinbase Wallet, etc.)
2. Register a username
3. Play free quiz rounds (no entry fee)
4. Answer timed quiz questions
5. Earn ETH rewards paid automatically via smart contracts

No staking. No long setup. Just connect → play → earn.

---

# 🚀 **Live on Base Mainnet!**

### Production Contracts

* **trivia-verseGame:** [View on BaseScan](https://basescan.org/address/0x7409Cbcb6577164E96A9b474efD4C32B9e17d59d)
* **USDC (Base Mainnet):** [View on BaseScan](https://basescan.org/token/0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913)
* **Network:** Base Mainnet (Chain ID: 8453)

---

---

# 🧠 **Features**

### 🌐 **Wallet Integration**

* Works with **any Web3 wallet** (MetaMask, Coinbase Wallet, WalletConnect)
* Instant balance updates
* Fast and cheap Base L2 transactions

### 💰 **Optional USDC Faucet**

* Each player can receive **10 USDC** once (testnet only)
* Enforced by smart contract
* Secure against multiple claims

### 🕹 **trivia-verseGame Gameplay**

* 10 random questions per game session
* Multiple-choice questions
* 5-minute time limit
* Responsive UI with smooth animations
* Questions selected via Chainlink VRF for fairness

### 🎁 **Reward Distribution**

* **FREE to play** (no entry fee)
* Earn **0.001 ETH per correct answer**
* Earn **0.005 ETH bonus** for perfect score (10/10)
* Earn up to **0.002 ETH speed bonus** for fast answers
* **Max reward per game: 0.017 ETH**
* Rewards distributed automatically via smart contract

### 🏆 **Leaderboard**

* Track top 100 players by total score
* Username registration system
* Weekly reward distribution for top 10 players
* Real-time rank updates

### 📱 **Built for All Devices**

* Responsive design
* Optimized for both desktop and mobile
* Smooth animations with Framer Motion
* Minimal steps to play

---

# 🏗 **Architecture**

## High-Level Flow

NEXT_PUBLIC_trivia-verse_GAME_V2_ADDRESS=0x...

```
Web3 Wallet → Register Username → Start Game → Answer Questions → Submit Answers → Claim ETH Rewards
```

## System Diagram

```
+------------------+      +----------------------+     +----------------------+
|  Frontend (Next) | <--> | trivia-verseGameV2.sol     | <-> | Chainlink VRF V2     |
+------------------+      +----------------------+     +----------------------+
         |                          |
         |                          |
         v                          v
+------------------+      +------------------+
|  Faucet.sol      |      | USDC Token       |
|  (Optional)      |      | (Base Mainnet)   |
+------------------+      +------------------+
```

---

# 🧩 **Tech Stack**

1. Update `contracts/script/Deploytrivia-verseGameV2.s.sol` with your subscription ID

* Solidity 0.8.20
* Foundry (Forge)
* OpenZeppelin Contracts
* Chainlink VRF V2
* Base Mainnet
* USDC (ERC20)
forge script script/Deploytrivia-verseGameV2.s.sol:Deploytrivia-verseGameV2 \

# TriviaVerse

TriviaVerse is a decentralized, blockchain-powered quiz and trivia platform built on the Base network. It enables users to play quiz rounds, answer questions, and earn real ETH rewards on-chain, all managed by secure smart contracts.

## Features

- Seamless Web3 wallet integration (MetaMask, Coinbase Wallet, WalletConnect)
- Fast, low-cost L2 transactions on Base
- Real ETH rewards distributed automatically
- Fair, random question selection via Chainlink VRF
- On-chain leaderboard and weekly rewards
- Responsive, modern frontend (Next.js, TypeScript)
- Open source and developer friendly

## Getting Started

### Prerequisites
- Node.js (v18+ recommended)
- npm or yarn
- Foundry (for smart contract development)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/carlton-source/trivia-verse.git
   cd trivia-verse
   ```
2. Install dependencies:
   ```bash
   cd contracts && npm install
   cd ../frontend && npm install
   ```

### Running the App

#### Smart Contracts
1. Compile contracts:
   ```bash
   cd contracts
   forge build
   ```
2. Deploy contracts (see scripts in contracts/script/ for examples).

#### Frontend
1. Start the development server:
   ```bash
   cd frontend
   npm run dev
   ```
2. Visit [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

- `contracts/` — Solidity smart contracts and deployment scripts
- `frontend/` — Next.js frontend application

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements, bug fixes, or new features.

## License

This project is licensed under the MIT License.
* Leaderboard tracking (top 100 players)

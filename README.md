# BOT
Bot for Quant Calculations

# 🐢 Green Turtle Arbitrage Bot – Project Overview

## 📘 Project Summary

The **Green Turtle Bot** is an intelligent, AI-enhanced arbitrage trading system designed for the Arbitrum blockchain. It monitors price discrepancies between multiple DEXes (e.g., Uniswap, SushiSwap) and exploits triangular arbitrage opportunities across WETH, USDC, and WBTC tokens.

This system:
- Uses **real-time Web3 on-chain price data** and **off-chain pricing from Kraken**.
- Executes profitable trades through a **single on-chain smart contract call**.
- Incorporates **Monte Carlo simulations** for profit volatility forecasting.
- Leverages an **LLM-based strategy layer** for adaptive, context-aware decision-making.
- Supports automatic **contract funding and profit sweeping** to wallet.

## ⚙️ Core Features

- 🧠 **AI-Augmented Strategy Layer**: LLMs (e.g., GPT) advise which routes to execute.
- 📈 **Monte Carlo Simulator**: Evaluates probabilistic outcomes to filter risky paths.
- 🔁 **Live Loop Execution**: Evaluates all supported arbitrage paths every 6 seconds.
- 🧪 **Off-Chain Profit Simulation**: Fast pre-check before spending gas.
- 🔐 **Smart Contract Execution**: Secure on-chain arbitrage settlement.
- 💸 **Auto Funding & Sweeping**: Deposit tokens in and retrieve profits out.

## 🚀 How to Use

### 1. **Install Dependencies**
```bash
pip install web3 python-dotenv requests numpy
```
### 2. **Configure Environment Variables**
```bash
Create a .env file with:
WALLET=0xYourWalletAddress
PRIVATE_KEY=YourPrivateKey
ARB_RPC_URL=https://your.rpc.url
CONTRACT_ADDRESS=0xYourContract
WETH=0xTokenAddr
USDC=0xTokenAddr
WBTC=0xTokenAddr
UNI_ROUTER=0xRouterAddr
SUSHI_ROUTER=0xRouterAddr
MIN_PROFIT_USD=1.0
```
### 3. **Run the Bot**
```bash
python Bot.py
```



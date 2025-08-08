# Solana HFT Copy Trading Bot

This project is a production-ready template for building Solana high-frequency bots that mirror Smart Money wallets in real-time across DEXs like Raydium AMM4, Meteora, and fallback to Jupiter routes.

## 🔧 Features
- Smart wallet mirroring using `logsSubscribe`
- Same-slot execution with `ComputeBudgetProgram`
- Multi-DEX instruction crafting (Raydium, Meteora, Jupiter)
- Modular exit strategies: principal withdrawal, partial PnL booking
- Metrics tracking: slot latency, dropped TXs, reorgs

## 🛠 Prerequisites
- Rust + Solana CLI installed
- RPC Node (preferably QuickNode or Helius)
- Private key with SOL for priority fees

## 🧪 Run
```bash
cargo run --release
```

## ⚙️ Configuration
Edit `.env`:
```env
RPC_URL=https://api.mainnet-beta.solana.com
SMART_WALLETS=wallet1,wallet2,...
FEE_MULTIPLIER=2.5
```

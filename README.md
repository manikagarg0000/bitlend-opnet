# bitlend-opnet

[README.md](https://github.com/user-attachments/files/25797765/README.md)
# ⚡ BitLend — DeFi Lending on Bitcoin L1 via OP_NET

> ETH/SOL-style DeFi lending, now on Bitcoin L1. Deposit BTC or OP_20 tokens, borrow stablecoins, earn yield — all powered by OP_NET.

![BitLend Preview](https://img.shields.io/badge/Network-OP__NET%20%C2%B7%20BTC%20L1-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Deploy](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge)

---

## 🗂️ Project Structure

```
bitlend-opnet/
├── public/
│   ├── index.html        ← Main app (entire frontend lives here)
│   ├── 404.html          ← Custom 404 page
│   └── robots.txt        ← SEO robots file
├── .github/
│   └── workflows/
│       └── deploy.yml    ← Auto-deploy to Vercel on git push
├── .gitignore
├── package.json
├── vercel.json           ← Vercel routing & headers config
└── README.md
```

---

## ✨ Features

- **4 Real Wallet Integrations** — OP_NET, Unisat, Xverse, OKX
- **Collateralized Lending** — Deposit BTC / OP_20 tokens as collateral
- **Live LTV Ratio** — Real-time loan-to-value tracking
- **Borrow Stablecoins** — OP_USDT & other OP_20 assets
- **Liquidation Engine** — Auto-liquidate below 82.5% threshold
- **Revenue Vault** — Interest fees → staker yield
- **TX Log** — Every action gets a TXID with OP_SCAN link
- **Live Dashboard** — Real-time balances, health factor, interest accrual

---

## 🚀 Quick Start (Local)

### Prerequisites
- [Node.js 18+](https://nodejs.org) installed
- A Bitcoin wallet extension installed in your browser (Unisat / Xverse / OKX / OP_NET)

### Steps

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/bitlend-opnet.git
cd bitlend-opnet

# 2. Install dependencies
npm install

# 3. Run locally
npm run dev

# 4. Open in browser
# → http://localhost:3000
```

> ⚠️ **Important:** Open via `http://localhost:3000` — NOT by double-clicking the HTML file.  
> Wallet extensions only inject into `http://` or `https://` pages, not `file://` pages.

---

## 📤 Deploy to Vercel

### Method 1 — Vercel CLI (Fastest, 2 minutes)

```bash
# Step 1: Install Vercel CLI globally
npm install -g vercel

# Step 2: Login to Vercel
vercel login
# → Opens browser, login with GitHub/Google/Email

# Step 3: Deploy from project root
cd bitlend-opnet
vercel

# 🔐 x402 Payment Gateway Video Paywall Demo

A complete demonstration of how to implement a **crypto payment gateway** using the **x402 payment protocol**.  
This project shows how to create a **video paywall** where users pay a small fee in **USDC** (on Base Sepolia or Base Mainnet) to unlock premium content.

Optimized for developers searching for:  
**x402 payment gateway • x402 crypto payments • x402 paywall • USDC paywall • Web3 monetization**

---

## 🚀 Features

- ⚡ **x402 Payment Gateway Integration** with `x402-express` middleware  
- 🔐 **Paywalled video endpoint** using crypto micro-payments  
- 🧩 **Client-side payment initiation** for x402 flows  
- 🧪 **Base Sepolia testnet support** for simple testing  
- 🌐 Minimal Express server—easy to extend into SaaS, API, or Web3 product  

---

## 📦 Prerequisites

- **Node.js v22+**
- **EVM wallet** with **USDC on Base Sepolia**

---

## 🛠 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/m4rcu5o/Coinbase-x402.git
```

### 2. Install dependencies
```bash
npm install
```

### 3. Configure your `.env` file  
Rename `.env.local` → `.env` and update:

```
WALLET_ADDRESS=your_ethereum_wallet_address
NODE_ENV=development
PORT=4021
```

This wallet receives all x402 payments.

### 4. Get Base Sepolia USDC  
- Visit: https://faucet.circle.com/  
- Select **Base Sepolia**  
- Request test USDC  

### 5. Start the server
```bash
npm run dev
```

### 6. Open your browser  
```
http://localhost:4021
```

---

## 🔍 How the x402 Payment Gateway Works

1. The server applies `x402-express` middleware to protect `/authenticate`  
2. When a user accesses the protected route, x402 triggers a **crypto payment request**  
3. User pays using USDC (via Base Sepolia or Base Mainnet)  
4. After successful payment, they are redirected to `/video-content`  
5. The paywalled video is now accessible

This demo can be extended into:  
- Paid courses  
- Premium media platforms  
- API monetization  
- SaaS paywalls  
- Micro-subscription systems  
- Developer tools with per-request billing  

---

## 🎛 Customizing

- **Change price:**  
  Edit `price` in `api/index.js`

- **Replace video:**  
  Modify `public/video-content.html`

- **Deploy on Base Mainnet:**  
  Update network config in `api/index.js`  
  → Requires CDP API keys  
  → Requires mainnet-compatible Facilitator  

---

## 📞 Contact  
For custom x402 gateway integrations or production-grade paywall systems:  
**Telegram:** https://t.me/idioRusty

---

⭐ If this project helps you, please **Star** the repo!  

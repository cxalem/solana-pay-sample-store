# Solana Pay Store Template

An educational Next.js template demonstrating how to integrate **Solana Pay** for accepting cryptocurrency payments in your e-commerce store.

## ✨ Features

- 🛍️ **Full E-commerce Store** - Product catalog, shopping cart, checkout flow
- 💳 **Solana Pay Integration** - Accept USDC payments with QR codes
- 📱 **Mobile Wallet Support** - Scan QR codes with any Solana wallet app
- ✅ **Payment Validation** - Verify transactions on-chain
- 💵 **USDC Payments** - Stable pricing with USD-pegged stablecoin
- 🎨 **Modern UI** - Built with Next.js 15, Tailwind CSS, and Shadcn UI
- 🔧 **TypeScript** - Fully typed codebase
- 📚 **Educational** - Well-documented code for learning

## 🚀 Quick Start

### 1. Install Dependencies

```shell
npm install
# or
pnpm install
```

### 2. Configure Environment

Create a `.env.local` file in the root directory:

```bash
# Your merchant wallet address (where payments will be received)
NEXT_PUBLIC_MERCHANT_WALLET=YourSolanaWalletPublicKeyHere

# Solana RPC endpoint (use devnet for testing)
NEXT_PUBLIC_RPC_URL=https://api.devnet.solana.com

# Base URL (optional, for API endpoints)
NEXT_PUBLIC_BASE_URL=http://localhost:3000
```

> **Testing**: Get devnet SOL from https://faucet.solana.com/

### 3. Start Development Server

```shell
npm run dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) and start accepting USDC payments!

> **Note**: Get devnet USDC from https://spl-token-faucet.com/?token-name=USDC-Dev

## 📖 Documentation

See **[SOLANA_PAY_SETUP.md](./SOLANA_PAY_SETUP.md)** for:
- Complete setup instructions
- Architecture overview
- Implementation details
- Code examples
- Troubleshooting guide

## 🏗️ Tech Stack

- **[Next.js 15](https://nextjs.org/)** - React framework
- **[Solana Pay](https://solanapay.com/)** - Payment protocol
- **[@solana/web3.js](https://solana.com/docs/clients/javascript)** - Solana SDK
- **[Gill](https://gill.site/)** - Solana wallet adapter
- **[Tailwind CSS](https://tailwindcss.com/)** - Styling
- **[Shadcn UI](https://ui.shadcn.com/)** - UI components
- **[TypeScript](https://www.typescriptlang.org/)** - Type safety

## 📁 Project Structure

```
/src/
├── lib/solana-pay/          # Solana Pay core utilities
├── hooks/                    # React hooks for payments
├── components/checkout/      # Checkout UI components
├── store/                    # Store logic (products, cart)
└── app/                      # Next.js app router
```

## 🎯 Learn More

- [Solana Pay Documentation](https://docs.solanapay.com/)
- [Solana Web3.js Guide](https://solana.com/docs/clients/javascript)
- [Next.js Documentation](https://nextjs.org/docs)

## 📝 License

Apache-2.0

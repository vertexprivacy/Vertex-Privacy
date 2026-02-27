# 🚀 LuminaZK - Quick Start Guide

## Setup Development Environment

### 1. Install Dependencies
```bash
npm install --legacy-peer-deps
```

**Note:** Use `--legacy-peer-deps` flag to handle peer dependency conflicts.

### 2. Configure Environment Variables (Optional)

Create `.env.local` file:
```env
# Optional: Better RPC performance
NEXT_PUBLIC_ALCHEMY_ID=your_alchemy_api_key

# Optional: More wallet options via WalletConnect
NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID=your_project_id
```

**Note**: App works without these - uses public RPCs as fallback!

### 3. Run Development Server
```bash
npm run dev
```

Open http://localhost:3000

## Test Wallet Connection

### Prerequisites
- Install MetaMask: https://metamask.io/
- Get test ETH: https://sepoliafaucet.com/ (for Sepolia testnet)

### Steps
1. Click "Connect Wallet" button
2. Select MetaMask (or any supported wallet)
3. Approve connection
4. Your address appears in button
5. Click address to switch networks or disconnect

## Features Implemented

✅ **Dark/Light Theme** - Toggle with Sun/Moon icon
✅ **Wallet Connection** - Connect Ethereum wallets (MetaMask, WalletConnect, etc.)
✅ **Multi-Chain** - Ethereum, Polygon, Arbitrum, Optimism, Base, Sepolia
✅ **Responsive Design** - Mobile, tablet, desktop optimized
✅ **ENS Support** - Display .eth names instead of addresses

## Project Structure

```
app/
  ├── layout.tsx          # Root layout with providers
  ├── page.tsx            # Landing page
  └── manage/
      └── page.tsx        # File management page

components/
  ├── web3-provider.tsx   # Wagmi + ConnectKit setup
  ├── wallet-button.tsx   # Custom wallet button
  ├── theme-provider.tsx  # Dark/light theme
  └── theme-toggle.tsx    # Theme toggle button

app/globals.css           # Global styles + theme variables
```

## Available Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run start    # Start production server
npm run lint     # Run ESLint
```

## Tech Stack

- **Next.js 16** - React framework
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Wagmi v2** - Ethereum React hooks
- **ConnectKit** - Wallet connection UI
- **Viem** - Ethereum TypeScript interface
- **TanStack Query** - Data fetching

## Branding

- **Name**: LuminaZK
- **Theme**: Dark green matrix-inspired
- **Default**: Dark mode
- **Colors**: Neon green (#72f2a0) on deep black

## Need Help?

- **Wallet Docs**: See `WALLET_WAGMI.md`
- **Theme Docs**: See theme variables in `app/globals.css`
- **Wagmi Docs**: https://wagmi.sh/
- **ConnectKit Docs**: https://docs.family.co/connectkit

---

Built with 💚 by the LuminaZK team

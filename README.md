# SUI-KSH Exchange

A web-app prototype for exchanging SUI and Kenyan shillings (KSh). The interface provides exchange quotes, transaction history, a dashboard, and account settings.

> **Prototype notice:** This project currently uses mock exchange rates, demo authentication, and simulated transaction and M-PESA processing. It does not submit transactions to the Sui blockchain or send real M-PESA payments. Should not be used to exchange real funds.

## Features

- SUI-to-KSh and KSh-to-SUI exchange interface
- Exchange-rate and historical-rate displays
- Transaction history with status, type, and search filters
- Dashboard with rate, liquidity-pool, and transaction statistics
- Price alert interface
- Demo sign-in and account settings for Sui wallet and M-PESA details
- Fee and slippage settings

## Tech stack

- React 18 and TypeScript
- Vite
- React Router
- Tailwind CSS
- Lucide icons and React Hot Toast

## Getting started

### Requirements

- Node.js and npm

### Install and run

```bash
npm install
npm run dev
```

Vite prints the local development URL in the terminal after the server starts.

## Available scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the development server |
| `npm run build` | Build the production app |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run ESLint |

## Current implementation status

Exchange rates and historical data are generated locally for demonstration. Authentication stores a mock user in browser local storage. Exchange and M-PESA processing are simulated in the frontend; the Sui wallet, smart-contract, price-oracle, and M-PESA Daraja integrations are not implemented.

Before handling real funds, the project would need audited on-chain contracts, wallet signing and transaction verification, a trusted rate source, secure backend services, and a properly configured M-PESA integration.

# 🧾 MultiWill – On-Chain Will Management (Template Version)

## 1. Project Title  
**MultiWill – Decentralized Multi-Recipient Will System**

A trustless, blockchain-powered inheritance system that allows users to create, manage, and claim digital wills entirely on-chain. Designed to work with any EVM-compatible network.

---
<img width="959" height="496" alt="image" src="https://github.com/user-attachments/assets/cf02555b-d40b-4916-96f9-90e1045d5c4c" />

## 2. Contract Address  

This template is not yet connected to a deployed contract.

- **Contract Address:** 0xF302134fbC6525bD0be4cA2aA040f3A5F9ff8492
  
- **Explorer Link:** https://coston2-explorer.flare.network/address/0xF302134fbC6525bD0be4cA2aA040f3A5F9ff8492
 

You can update these once the smart contract is deployed.

---

## 3. Description  

**MultiWill** is a decentralized inheritance protocol enabling users to create multiple wills directly from their crypto wallet. Each will assigns a specific amount of native tokens to a chosen recipient. The contract securely locks the funds and ensures that only the designated recipient can claim them.

The system is entirely on-chain, removing dependence on centralized institutions, legal intermediaries, or custodial platforms. All interactions occur through smart contract calls, ensuring predictable, transparent, and censorship-resistant execution.

This repository includes:  
- A **contract interaction hook** (`useWillContract`) built with Wagmi + Viem  
- A **sample UI** demonstrating live reading of on-chain state and transaction handling  
- Clean architecture ready for integration into any Next.js or React project  

---

## 4. Features  

### 🔐 Fully Decentralized Will Creation  
- Create wills directly from the user’s wallet  
- No middlemen, custodians, or trust requirements  
- Funds are locked in the smart contract until claimed  

### 🧾 Unlimited Wills Per User  
- Each address can create multiple wills  
- Enables distribution across family, friends, DAOs, communities, or multiple wallets  

### 💰 Native Token Funding  
- Wills store native blockchain tokens (e.g., FLR, ETH, MATIC, BNB)  
- Amount sent during `createWill` becomes the inheritance balance  

### 🎯 Recipient-Only Claiming  
- Only the assigned recipient can call `claimWill`  
- Once claimed, the will is marked as completed to prevent double claims  

### 📊 On-Chain Transparency  
- Anyone can query:  
  - Contract balance  
  - Wills created by a user  
  - Will details (recipient, amount, and status)  
- No hidden logic, everything is verifiable on-chain  

### ⚙️ Developer-Friendly Hook  
Included hook (`useWillContract`) provides:  
- Contract reads (balance, counts)  
- Writes (create, claim)  
- Loading + confirmation states  
- Error handling  
- Wallet gating  
- Clean TypeScript types  

### 🖥️ Sample UI Included  
The provided UI (`components/sample.tsx`) demonstrates:  
- Wallet connection with Wagmi  
- Validations (recipient address, input states)  
- Real-time transaction feedback  
- Create and claim operations  
- Modern TailwindCSS-styled interface  

---

## 5. How It Solves the Problem  

### ❌ The Problem  
Inheritance in traditional systems is:  
- Slow, centralized, and jurisdiction-dependent  
- Opaque, with little visibility for beneficiaries  
- Not designed for digital assets  
- Dependent on lawyers, custodians, or intermediaries  
- Difficult across borders  
- Vulnerable to disputes or mismanagement  

For blockchain assets, the situation is even worse:  
- Private keys cannot be easily transferred  
- Exchanges and custodial services introduce risks  
- No automated mechanisms exist for allocation  

---

### ✅ The MultiWill Solution  

#### 1. Automated Smart Contract Logic  
Inheritance rules are enforced by code:  
- Recipients must match the stored address  
- Amounts cannot be altered after creation  
- Claims are atomic, transparent, and secure  

No human intervention required.

#### 2. Transparent, Auditable State  
All wills and balances are recorded publicly on-chain:  
- Beneficiaries can verify their allocation  
- No need for legal documents or centralized servers  
- Ideal for dashboards, analytics, or advanced estate-planning dApps  

#### 3. Perfect for Digital Assets  
Built natively for blockchain tokens:  
- Eliminates reliance on centralized exchanges  
- Direct wallet-to-wallet transfers  
- Universally accessible, globally consistent  

#### 4. Easy Integration Into Any dApp  
The contract structure and ABI are minimal, clear, and composable.  
Developers can extend the system by adding:  
- Timelocks  
- Proof-of-life mechanisms  
- Oracles  
- Social recovery systems  
- Multi-executor systems for advanced inheritance  

#### 5. Useful for Real and Educational Projects  
This template offers:  
- Production-ready architecture  
- Clean React/Wagmi integration  
- A great starting point for testnet deployments, hackathons, or real products  

---

## 📌 Summary  

**MultiWill** introduces a simple, powerful, and decentralized way to manage digital inheritance.  
Whether used for personal estate planning, DAO-driven distributions, or educational demos, the system provides:

- Transparency  
- Security  
- Automation  
- Developer extensibility  

This repository includes the complete foundation to build a fully functional digital inheritance dApp.



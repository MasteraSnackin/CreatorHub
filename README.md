# CreatorHub

A full-stack Web3 platform integrating eight leading blockchain and decentralized technologies for the Encode London Hackathon. CreatorHub enables seamless interaction with Arbitrum, Concordium, Envio, Story Protocol, Livepeer, Openfort, Hakflow, and Neo—all through a unified, modular interface.

## Catch free creator
https://youtu.be/0OaoySgCJn0


## CreatorHub The Web3 Antidote
https://youtu.be/tPVdICxnEvc
  
**Data Flow Diagram level 0 Context Diagram**
<img width="891" height="490" alt="Level 0 Context Diagram" src="https://github.com/user-attachments/assets/d9ff8a29-9bd4-48ad-abf3-8ade75b47d3a" />


## Table of Contents

- [Features](#features)
- [Quick Start](#quick-start)
- [Architecture](#architecture)
- [Module Integration](#module-integration)
- [Deployment](#deployment)
- [Demo Deliverables](#demo-deliverables)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

  
**Sequence Diagram**
  <img width="2880" height="788" alt="Sequence Diagram" src="https://github.com/user-attachments/assets/723ce7f4-ea51-4aa6-904e-c99956fb4c9a" />


## Features
- **Unified Web3 Dashboard**: Manage bounties, identities, payments, and media across multiple chains and protocols.
- **Modular SDK Integration**: Each supported technology (Arbitrum, Concordium, Envio, Story Protocol, Livepeer, Openfort, Hakflow, Neo) has a dedicated React hook and backend module.
- **Cross-Chain Identity**: Leverage Concordium for decentralized identity and Openfort for seamless login.
- **Decentralized Media**: Integrate Livepeer for video streaming and Story Protocol for IP registration.
- **Smart Contract Security**: Built-in Hakflow audits for all deployed contracts.
- **Scalable Backend**: Node.js API with Rust microservices and Envio-HyperIndex for real-time blockchain data.
- **Easy Deployment**: One-command Docker Compose setup for backend, Vercel for frontend, and testnet support.

  
**Data Flow Diagram level 2 detailed flows**
<img width="1039" height="709" alt="Data Flow Dirgram level2 detailed flows" src="https://github.com/user-attachments/assets/ecec1f48-e4ff-430a-883d-2bfc697bb2c3" />

Core Features
- **AI-Driven Monetization:** Creators issue, license, and receive royalties for works, with on-chain proof and programmable payout flows.
- **Verified Identity:** Users and creators undergo privacy-preserving ID checks for compliance and security, leveraging Concordium.
- **Integrated Wallet Experience:** Users can seamlessly onboard and use wallets with no Web3 knowledge needed, powered by Openfort.
- **Automated Payments:** AI agents on Arbitrum enable micro- and macro-payments autonomously between verified participants.
- **IP Security: On-chain registration of content via Story Protocol ensures verified ownership, instant licensing, and dispute resolution.
- **Video Streaming and Content Delivery:** Livepeer provides scalable infrastructure for streaming, on-demand, and AI-enhanced media.
- **Real-time Analytics:** Envio’s HyperIndex facilitates instant access to platform, content, and user metrics across multiple blockchains.
- **Smart Contract Security:** All contracts are reviewed/audited using Hakflow, ensuring production-level safety and hack-resistance.
- **Educational Material:** Tutorials, onboarding, and integration guides are generated on Neo SpoonOS, powering new developer entry.

**Data Flow Diagram level 1 Main Processes**
<img width="969" height="776" alt="Data Flow Diagram level1 main processes " src="https://github.com/user-attachments/assets/5c20a458-37d8-4d97-ba53-852bd6b9a2e7" />

Technical Depth
- **Monorepo Architecture:** All code, contracts, and documentation housed in one GitHub repository, maximizing synergy and meeting each bounty’s submission criteria.
- **SDK-First Development:** Utilization of SDKs where available (Story, Openfort, Arbitrum, etc.) for rapid, robust feature rollout.
- **Multi-language Stack:** TypeScript, Rust, Solidity, and Python for broad compatibility and maximum feature set utilization.
- **Simultaneous Testnets:** Use of Arbitrum Sepolia, Concordium testnet, and Story/Aeneid for sandboxing before mainnet deployment.
- **CI/CD Pipeline Integration:** Automated testing and security analysis via Hakflow and other static/dynamic analysis tools.
- **User Experience Focus:** OAuth and social logins reduce onboarding friction; dynamic dashboards provide actionable insights.
- **Video Workflows:** Integration with Livepeer’s APIs for upload, processing, and dynamic streaming tied to on-chain user privileges.
- **Content Registration Flows:** All user-generated content is funneled through Story Protocol SDK to mint NFTs and assign licenses at upload time.
- **Agentic Payments:** AI modules connect to Arbitrum payment rails, supporting programmable payouts, splits, or pay-per-insight/distribution.


## Quick Start

```bash
# Clone the repository
git clone https://github.com/your-username/creatorhub.git
cd creatorhub

# Frontend setup
npm install
npm run dev

# Backend setup
cd backend
npm install
npm start

# Envio Data Layer
git clone https://github.com/enviodev/hyperindex
cd hyperindex && npm install && npm run build

# Rust dependencies (Concordium)
rustup install 1.73.0
cargo install cargo-concordium
docker-compose up -d

# See individual module READMEs for further setup.
```

## Architecture

- **Frontend**: Next.js 14, TypeScript, TailwindCSS, modular React hooks for all SDKs
- **Backend**: Node.js Express API, Rust microservice for Concordium, Envio-HyperIndex data streaming
- **Smart Contracts**: Solidity (Arbitrum), Rust Wasm (Concordium), Hakflow security audits

## Sequence Diagram - IP Registration Flow
<img width="1221" height="805" alt="Sequence Diagram - IP Registration Flow" src="https://github.com/user-attachments/assets/35338e16-b133-4fdf-ac7d-07d76b78aff3" />


## Identity Verification Flow
<img width="1327" height="750" alt="Sequence Diagram - Identity Verification Flow" src="https://github.com/user-attachments/assets/2811538b-4a07-4a1f-8c91-64bcc1666ba2" />


## Module Integration

Each supported technology module includes detailed documentation and example integrations. Refer to the official documentation and GitHub starter kits for each module for SDK and API integration.

## Deployment

1. **Configure Environment**: Set all required API keys and endpoints in `.env` (Openfort, Livepeer Studio, Arbitrum RPC, Concordium endpoint, etc.)
2. **Security Scan**: Run Hakflow pre-submission scan and commit the security report.
3. **Publish**: Push to GitHub (public repo) with README, architecture diagram, and demo video links.
4. **Deploy**: Frontend via Vercel, backend via Docker Compose, smart contracts to Arbitrum Sepolia testnet.


## Contributing

We welcome contributions! Please fork the repository, create a feature branch, and submit a pull request. For major changes, open an issue first to discuss.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact

For questions or support, open an issue on GitHub or contact the project maintainers directly.

---

*Replace placeholder links and images with actual project assets before public release.*

<div align="center">

# 🌌 Q-AI Chain Protocol
### *Quantum-Secure AI-Powered Trust Protocol*

[![Stability: Stable](https://img.shields.io/badge/Status-Protocol--Ready-brightgreen?style=for-the-badge&logo=git&logoColor=white)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-blue.svg?style=for-the-badge&logo=github&logoColor=white)]()
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=for-the-badge&logo=apache&logoColor=white)](LICENSE)

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=150&section=header&text=Q-AI%20Chain&fontSize=50&fontAlignY=38&animation=twinkling&desc=Next-Gen%20Decentralized%20Trust&descAlignY=60" />

**Q-AI Chain** is a state-of-the-art modular protocol for identity verification, transaction security, and fraud prevention in a post-quantum world. 

[**Explore Setup Guide**](SETUP_GUIDE.md) | [**View SDK Docs**](sdk/README.md) | [**Architecture**](docs/architecture.md)

</div>

---

## 💎 Core Pillars

<table align="center">
  <tr>
    <td align="center"><h3>🧠 AI Engine</h3></td>
    <td align="center"><h3>🛡 Quantum Security</h3></td>
    <td align="center"><h3>⛓ Blockchain Trust</h3></td>
  </tr>
  <tr>
    <td><strong>Isolation Forest</strong> anomaly detection detects fraud before it happens.</td>
    <td>Integrated with <strong>Dilithium2</strong> and <strong>Kyber</strong> for PQ resistance.</td>
    <td>Immutable anchoring of trust scores and identities on-chain.</td>
  </tr>
</table>

---

## 🏗 System Architecture

```mermaid
graph TD
    classDef default fill:#1f2937,stroke:#3b82f6,stroke-width:2px,color:#fff;
    classDef highlight fill:#3b82f6,stroke:#fff,stroke-width:2px,color:#fff;
    classDef database fill:#10b981,stroke:#047857,stroke-width:2px,color:#fff;

    A[📱 Client App / SDK]:::default --> B[⚡ FastAPI Gateway]:::highlight
    B --> C{🧠 AI Engine}:::default
    C -->|Anomaly| D[⚠️ Manual Review]:::default
    C -->|Pass| E[🔐 PQC Signature]:::default
    E --> F[⛓ Blockchain Relayer]:::default
    F --> G[(🌐 Ethereum Sepolia)]:::database
    B --> H[(🛡 Quantum Vault)]:::database
    B --> I[(💾 Postgres/Redis)]:::database
```

---

## 🚀 Key Features

* ✨ **PQC-DID Registry**: Decentralized identities secured by Post-Quantum Cryptography.
* ⚡ **Real-Time Risk Scoring**: Dynamic risk assessment for every transaction.
* 🔄 **Relayer Pathing**: Advanced on-chain anchoring with nonce-management and idempotency.
* 🛠 **Developer First**: Fully typed FastAPI backend and a clean, lightweight JS SDK.

---

## 📂 Protocol Components

| Module | Description | Path |
| :--- | :--- | :--- |
| 📜 **Contracts** | Solidity registries for Identity, Transactions, and Risk | `contracts/` |
| ⚙️ **Backend** | Protocol logic featuring Dilithium/Kyber integration | `backend/` |
| 🧠 **AI Engine** | Local AI artifacts for deterministic fraud detection | `ai-engine/` |
| 🎨 **Frontend** | Premium Tailwind-powered dashboard for network monitoring | `frontend/` |
| 📦 **SDK** | Ethers.js v6 abstraction for third-party service integration | `sdk/` |
| 🐳 **Infra** | Dockerized environment for instant local deployment | `infra/` |

---

> [!TIP]
> **Getting Started?**
> The safest way to deploy is through our specialized infrastructure! Check the `infra/` folder for one-command deployment.

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer" />
  <p>Developed for a <strong>secure, decentralized, and intelligent future</strong>.</p>
</div>

# pollingapp_x

*Empowering secure, transparent elections for everyone.*

![last-commit](https://img.shields.io/github/last-commit/ixgnoy/DApp_pollingapp)
![repo-top-language](https://img.shields.io/github/languages/top/ixgnoy/DApp_pollingapp)
![repo-language-count](https://img.shields.io/github/languages/count/ixgnoy/DApp_pollingapp)
![Visitors](https://visitor-badge.laobi.icu/badge?page_id=ixgnoy.DApp_pollingapp)

---

## 🛠️ Built with the tools and technologies:

![JSON](https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)
![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GNU Bash](https://img.shields.io/badge/GNU%20Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![React Bootstrap](https://img.shields.io/badge/React%20Bootstrap-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Ethers](https://img.shields.io/badge/Ethers.js-4C51BF?style=for-the-badge&logo=ethereum&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![IPFS](https://img.shields.io/badge/IPFS-65C2CB?style=for-the-badge&logo=ipfs&logoColor=white)
![Chainlink](https://img.shields.io/badge/Chainlink%20Oracle-375BD2?style=for-the-badge&logo=chainlink&logoColor=white)

---
🔍 Introduction
This is a Web3-based decentralized voting application built with Ethereum, Solidity, Hardhat, React, and IPFS. It allows users to securely cast votes through a smart contract deployed on the Ethereum blockchain. IPFS is used to store immutable records and assets off-chain, and Oracle integration supports real-world event validation on Layer 2.

🧱 Tech Stack
Frontend: React, JavaScript, Bootstrap

Blockchain: Solidity, Hardhat, Ethereum (RPC)

Off-chain Storage: IPFS

Oracle: Chainlink / L2 Oracle Protocols

Smart Contract Deployment & Testing: Hardhat

Wallet Integration: MetaMask / Web3-compatible wallets

✨ Features
Admin and Voting Panels

Smart Contract-based vote casting

Event listening for VoteCast

Off-chain IPFS-based voter proof archival

Oracle-integrated real-world data validation

L2 interoperability and gas optimization

Secure, transparent election process

📦 IPFS Integration
What is IPFS?
IPFS (InterPlanetary File System) is a distributed system for storing and accessing files, websites, and data in a peer-to-peer network.

Why use IPFS in this DApp?

Decentralized file storage

Permanent, tamper-proof data

Cryptographic hashes for integrity

Reduces gas by storing large data off-chain

Use cases in this project:

Store voter identities, candidate manifestos, or election certificates as IPFS hashes

Retrieve and display IPFS content via https://ipfs.io/ipfs/{CID}

Example flow:

Admin uploads a manifesto PDF or campaign media to IPFS

IPFS returns a content hash (CID)

CID is stored in the blockchain smart contract

Frontend fetches the file via public IPFS gateways

🛰️ Layer 2 Blockchain Oracle Integration
What are Oracles?
Oracles bridge the gap between on-chain and off-chain data. They fetch, verify, and relay external data (like timestamps, identity checks, or event triggers) into smart contracts.

Why Oracle + L2?

Lower gas fees (via L2 solutions like Arbitrum/Optimism)

Real-world conditional logic (e.g., “voting closes 10 minutes after real-world event X”)

External API or timestamp validation

Resilience and scalability

Use cases in this project:

Validate a voter’s eligibility via an external system

Trigger election closure after Chainlink timestamp

Query real-time regional results (aggregated via Oracle feed)

🗺️ Architecture Diagram
<img src="Architecture diagram/diagram.png"/>

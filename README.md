# pollingapp_x

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

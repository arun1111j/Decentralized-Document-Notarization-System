# Decentralized Document Notarization System

A blockchain-based platform that provides secure, transparent, and cost-effective document notarization using Ethereum smart contracts and IPFS decentralized storage.

## About

The Decentralized Document Notarization System addresses the limitations of traditional notarization by leveraging blockchain technology to create an immutable, trustless framework for document verification. This system eliminates centralized authorities, reduces costs, and provides global accessibility while maintaining document privacy through cryptographic hashing.

The platform implements a multi-tier architecture with React frontend, Spring Boot backend, Ethereum smart contracts, and IPFS storage. It features a sophisticated notary management system with staking mechanisms, automated slashing for malicious actors, and real-time verification capabilities.

## Features

- **Immutable Document Registration**: Cryptographic hashing and blockchain timestamping for undeniable proof of existence
- **Multi-Notary Verification**: Distributed verification system with reputation-based notary selection
- **Economic Security Model**: Staking and slashing mechanisms to ensure participant accountability
- **Hybrid Storage Architecture**: IPFS for document storage + Blockchain for proof storage
- **Real-time Verification**: Instant document integrity verification with comprehensive audit trails
- **Role-Based Access Control**: Separate interfaces for Document Owners, Notaries, and Verifiers
- **Gas-Optimized Smart Contracts**: Efficient Solidity code with reentrancy protection

## Requirements

### Hardware Requirements
* **Development**: Intel Core i5 (8th Gen) or equivalent, 8GB RAM, 256GB SSD
* **Production**: Multi-core processor (Xeon/EPYC), 16GB RAM, 500GB SSD

### Software Requirements
* **Frontend**: React.js v18+, HTML5, CSS3, JavaScript ES6+, Web3.js/Ethers.js
* **Backend**: JDK 17+, Spring Boot v3.x, Maven v3.6+
* **Smart Contracts**: Solidity v0.8.x, Hardhat/Truffle framework
* **Blockchain**: Ethereum Sepolia Testnet/Mainnet, Infura/Alchemy node service
* **Database**: MySQL v8.0 or PostgreSQL v13+
* **Storage**: IPFS (Kubo daemon) with Pinata/Infura pinning service
* **Web3 Wallet**: MetaMask browser extension

## System Architecture

**Figure 2.1: Decentralized Notarization Platform Architecture**

<img width="751" height="615" alt="image" src="https://github.com/user-attachments/assets/42444d27-e8fe-4d45-a4aa-0b6da753838a" />

The system follows a layered architecture as shown in Figure 6.2:
- **Presentation Layer**: React frontend for user interaction
- **Application Layer**: Spring Boot backend for business logic orchestration
- **Data Layer**: Hybrid storage with SQL database, IPFS, and Ethereum blockchain
- **Identity Layer**: Web3 wallets for decentralized authentication

## Workflow

### Document Upload and Notarization Process
**Figure 7.1: Document Upload and Notarization Request Flowchart**

<img width="556" height="696" alt="image" src="https://github.com/user-attachments/assets/16ab4c27-d309-434d-8771-e81cadc45d27" />

The document lifecycle begins with upload, hashing, and IPFS storage, followed by notary verification and blockchain recording.

### Notary Verification Process
**Figure 7.2: Notary Verification Process Flowchart**

<img width="401" height="926" alt="image" src="https://github.com/user-attachments/assets/67abe924-88a1-4540-bb42-efc636fb72b1" />

Registered notaries review pending requests, verify documents, and execute smart contract functions for on-chain recording.

### Document Verification Process
**Figure 7.3: Document Verification Flowchart**

<img width="438" height="1002" alt="image" src="https://github.com/user-attachments/assets/cf586135-bf47-4f56-8118-bd69149775e8" />

Any user can verify document integrity by comparing computed hashes with blockchain records and validating IPFS content.

## System Design

### Use Case Diagram
**Figure 7.4: Use Case Diagram**

<img width="839" height="986" alt="image" src="https://github.com/user-attachments/assets/bb04bef4-9530-4759-ad44-7f2b76ab7f86" />

Shows interactions between Document Owners, Notaries, Verifiers, and System Administrators.

### Class Diagram
**Figure 7.5: Class Diagram**

<img width="784" height="738" alt="image" src="https://github.com/user-attachments/assets/3e30cb68-c60f-45aa-b13b-842f05f674b8" />

Illustrates the object-oriented design with entities like User, Document, Notarization, and their relationships.

### Sequence Diagram
**Figure 7.6: Sequence Diagram - Document Notarization**

<img width="685" height="329" alt="image" src="https://github.com/user-attachments/assets/37987394-96f3-4961-9c79-cc52fd0bf393" />

Demonstrates the chronological flow of messages between system components during notarization.

### Activity Diagram
**Figure 7.7: Activity Diagram - Complete Notarization Workflow**

<img width="659" height="526" alt="image" src="https://github.com/user-attachments/assets/523cafbe-67aa-496b-bbf5-e26f00fe483b" />

Provides a comprehensive view of the parallel and sequential activities in the notarization process.

## Output

### Document Verification System Flow
**Figure 6.1: Document Verification System Flowchart**

<img width="537" height="409" alt="image" src="https://github.com/user-attachments/assets/fbcc2fc2-f56c-4bb0-9cfa-be24fcb61508" />

Shows the end-to-end process from document submission to verification result.

### System Architecture Overview
**Figure 6.2: System Architecture Pyramid**

<img width="777" height="478" alt="image" src="https://github.com/user-attachments/assets/f78aa072-a823-40f2-a09b-be6cfe2d6f87" />

Illustrates the layered architecture with clear separation of concerns.

### Code Implementation Examples

**Figure 9.1: Smart Contract Snippet (Document Notarization)**

<img width="722" height="422" alt="image" src="https://github.com/user-attachments/assets/1c9d7821-e71c-400f-bc12-f173700dfb46" />

Core Solidity function handling document notarization with staking checks and event emission.

**Figure 9.2: Backend Snippet (Spring Boot Service)**

<img width="728" height="521" alt="image" src="https://github.com/user-attachments/assets/fdf94bff-e6f3-4901-bf36-117880b11ae2" />

Service method using Web3j to interact with Ethereum smart contracts.

**Figure 9.3: Frontend Snippet (React with Ethers.js)**

<img width="709" height="537" alt="image" src="https://github.com/user-attachments/assets/0aa720ac-4c7f-4ae9-9753-29472d573de1" />

React component handling MetaMask integration and transaction initiation.

**System Performance Metrics:**
- Document Upload & Hashing: ≤ 30 seconds
- Notarization Workflow: ≤ 2 minutes
- Document Verification: ≤ 5 seconds
- API Response Latency: ≤ 500ms
- System Uptime: 99.5%

## Results and Impact

The Decentralized Document Notarization System successfully demonstrates a viable alternative to traditional notarization, providing:

- **Enhanced Security**: Cryptographic proof of document integrity through blockchain immutability
- **Cost Reduction**: Elimination of intermediary fees through decentralized verification
- **Global Accessibility**: Borderless document verification capabilities
- **Transparency**: Publicly auditable notarization records without compromising document privacy
- **Trust Minimization**: Self-executing smart contracts replace centralized trust models

This project establishes a foundation for future developments in decentralized trust services and contributes to the broader adoption of blockchain technology in legal and business applications.

## Articles Published / References

1. Nakamoto, S. (2008). Bitcoin: A peer-to-peer electronic cash system.
2. Buterin, V. (2014). A next-generation smart contract and decentralized application platform.
3. Benet, J. (2014). IPFS-content addressed, versioned, p2p file system.
4. Atzei, N., Bartoletti, M., & Cimoli, T. (2017). A survey of attacks on ethereum smart contracts.
5. Rani, P., Sachan, R. K., & Kukreja, S. (2025). BT-CNV: A distributed and decentralized solution for certificate notarization and verification for academia using public blockchain.
6. Han, J., & Son, Y. (2025). Design and implementation of a decentralized document management system.

## License

This project is licensed under the GNU-3.0 License - see the LICENSE file for details.

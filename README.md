# 🧭 Web3 Project Roadmap & Checklist

## 🪜 PHASE 1 — Foundations (Theory & Setup)
🎯 *Goal: Understand the basics and set up your tools.*

- [ ] Understand blockchain basics (blocks, consensus, immutability)
- [ ] Learn about private/public keys and MetaMask wallets
- [ ] Understand Ethereum, EVM, gas, and transactions
- [ ] Install MetaMask and get Sepolia testnet ETH
- [ ] Set up VS Code, Node.js, and npm
- [ ] Learn Solidity syntax via [solidity-by-example.org](https://solidity-by-example.org)

---

## ⚙️ PHASE 2 — Build Your First Smart Contract
🎯 *Goal: Write and deploy a simple Solidity contract.*

- [ ] Install Hardhat and initialize a project (`npx hardhat init`)
- [ ] Write a simple contract (Greeting, Voting, or Todo List)
- [ ] Test the contract locally (`npx hardhat test`)
- [ ] Deploy to **Sepolia testnet** using Alchemy or Infura
- [ ] Verify contract on [Sepolia Etherscan](https://sepolia.etherscan.io) (optional)
- [ ] Interact with contract via Remix or Hardhat scripts

**Example contract:**
```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.24;

contract Greeting {
    string public message = "Hello Web3!";
    function setMessage(string calldata newMessage) external {
        message = newMessage;
    }
}

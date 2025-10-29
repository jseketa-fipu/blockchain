# Phase 1 — Foundations (Checklist)
Web3 application is a web application that interacts with a blockchain.

- [ ] Understand core concepts (accounts vs. wallets, networks, gas, nonce, chain ID, tokens, events/logs, explorers)
      - accounts vs. wallets
        - account - on-chain identity with an address and a balance
          - types of accounts:
            - EOA (*E*xternally *O*wned account) is controlled by a private key owned by you
            - a *contract account* runs code and is controlled by its contract logic      
        - wallet - off-chain tool/app that manages keys and signs transactions for one or more accounts
        
      - networks  
        - mainnet - real money
        - testnets (e.g. Sepolia) - play money for development

      - gas
        - fee paid to run code
        - Gas price * gas used = fee (in ETH)

      - nonce
        - per-account transaction counter to prevent replay and define order

      - chain ID
        - unique ID per network (Sepolia = 11155111) to stop cross-chain replay

      - tokens
        - native coin (ETH) vs. ERC-20 tokens (standardized contracts)

      - events/logs
        - contract emits events, which are indexed and easy to read on explorers

      - block explorers
        - websites (etherscan-style) showing blocks, transactions, logs, and contract code

- [ ] Install prerequisites (Node.js LTS, Git, MetaMask, RPC provider account)
- [ ] Initialize repo (git, `npm init`, `.gitignore`, `README.md`)
- [ ] Create `.env.example` and `.env` with `PRIVATE_KEY`, `RPC_URL`, `CHAIN_ID`
- [ ] Set up MetaMask (new test wallet, add Sepolia `11155111`, lock when not in use)
- [ ] Get test ETH from a faucet and confirm on explorer
- [ ] Verify RPC URL works (store in `.env`)

- [ ] **Choose ONE toolchain — Hardhat**
  - [ ] Install Hardhat + toolbox + dotenv
  - [ ] Compile a sample contract
  - [ ] Start local node
  - [ ] Deploy locally
  - [ ] Configure Sepolia network (RPC + private key)
  - [ ] Deploy to Sepolia and record the address
  - [ ] (Optional) Verify source on explorer

- [ ] **Interact with the contract**
  - [ ] Read a public variable (e.g., `count`) via script/`cast call`
  - [ ] Send a write transaction (e.g., `increment()`) via script/`cast send`
  - [ ] Confirm transaction, gas used, and events on the explorer

- [ ] **Repo hygiene**
  - [ ] Commit minimal structure (`contracts/` or `src/`, `scripts/`, config, `README.md`, `.env.example`, `.gitignore`)
  - [ ] Add npm scripts for build/test/deploy (or Foundry equivalents)
  - [ ] Keep secrets out of Git

- [ ] **Security basics**
  - [ ] Never commit seed phrases / private keys
  - [ ] Use a throwaway test wallet
  - [ ] Lock MetaMask after use

- [ ] **Done criteria**
  - [ ] Can explain gas, nonce, and chain ID
  - [ ] MetaMask funded on Sepolia
  - [ ] Contract deployed to Sepolia (address recorded)
  - [ ] Read/write interactions succeed and are visible on explorer
  - [ ] Repo contains clear run steps and env requirements

- [ ] **Troubleshooting**
  - [ ] INSUFFICIENT_FUNDS → get more test ETH
  - [ ] Nonce too low → wait or bump nonce
  - [ ] Invalid chain ID → fix config/network
  - [ ] ABI/address mismatch → verify contract name/address/ABI

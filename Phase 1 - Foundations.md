** Phase 1 — Foundations (Checklist) **

- [ ] Understand core concepts (accounts vs. wallets, networks, gas, nonce, chain ID, tokens, events/logs, explorers)
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
  - [ ] Send a write tx (e.g., `increment()`) via script/`cast send`
  - [ ] Confirm tx, gas used, and events on the explorer

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

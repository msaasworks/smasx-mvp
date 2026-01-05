# SMASX Protocol: MVP Verifier

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Status](https://img.shields.io/badge/status-development-yellow.svg) ![Solana](https://img.shields.io/badge/network-devnet-purple)

**The First Privacy-Preserving Airdrop Optimization Layer on Solana.**

This repository contains the MVP logic for the **"Proof of Knowledge"** verification engine described in the [SMASX Whitepaper v1.4](https://smasx.msaasworks.com).

## 🚧 Status: Under Development
The core logic for the off-chain `solana-py` verifier is currently being migrated from our private testing environment to this public repository.

### Technical Roadmap
- [x] **Phase 1:** Wallet Age Verification Logic (Python 3.9+)
- [ ] **Phase 2:** hCaptcha Integration Module
- [ ] **Phase 3:** Anchor Smart Contract Hook (Devnet)

## Usage (Preview)
```python
# Coming soon:
from smasx.verifier import check_wallet_age

def verify_user(wallet_address):
    # SMASX Protocol: Checks if wallet is >30 days old to prevent Sybil attacks
    return check_wallet_age(wallet_address, min_days=30)

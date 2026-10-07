# Foundry Account Abstraction

A lightweight Foundry starter for experimenting with account abstraction patterns in Solidity. This repository provides the project scaffold and environment setup needed to explore programmable accounts, wallet logic, and smart-contract account design in an EVM-first workflow.

## What the product does
This project is intended to serve as a base for building account abstraction experiments. Instead of depending only on externally owned accounts (EOAs), the setup is designed to support contract-based wallet patterns that can execute logic, validate custom rules, and manage programmable transaction flows.

The current repository is intentionally minimal and acts as a starting point for experimenting with account abstraction concepts in Foundry.

## The problem it solves
Standard EOAs are limited because they cannot encode complex validation logic, cannot easily recover from mistakes through programmable execution paths, and do not offer flexible wallet behaviors by default. Account abstraction aims to solve this by allowing smart contracts to act as accounts.

This project creates a clean environment for exploring that design space, with a test-first workflow using Foundry.

## My specific contribution
This repository establishes the Foundry project layout and the supporting dependency setup needed for account abstraction experiments. It includes the base configuration required to compile, test, and extend the project for more advanced smart-account logic.

## Architecture
The repository follows a standard Foundry structure:

- `src/` — Solidity source files for the protocol or experiment
- `script/` — deployment scripts and helper logic
- `test/` — tests for validating behavior
- `lib/` — external dependencies and libraries
- `foundry.toml` — Foundry configuration and project settings

At the current stage, this project is a minimal template rather than a full production-ready account abstraction wallet. It is designed to be expanded with custom account logic, validation flows, and execution models.

## Technologies
- Solidity
- Foundry
- Forge
- EVM-based smart contract design
- OpenZeppelin-compatible dependency patterns
- Standard Foundry workflows for testing and deployment

## Important technical decisions
- Foundry is used to keep the workspace fast, portable, and easily testable.
- The repository is intentionally lightweight so that account abstraction experiments can be added without unnecessary infrastructure.
- The project follows a modular layout, making it easy to add new smart-account patterns and validation logic.
- The setup prioritizes clarity and flexibility over production-scale implementation details.

## Key features
- Clean Foundry scaffold for Solidity experimentation
- Dependency-ready project for account abstraction work
- Easy extension for smart-account logic
- Fast compile/test flow using Foundry tooling
- Minimal but reusable project structure

## Screenshots
No screenshots are included in the repository at this stage.

## Live demo
No live demo or deployed application is currently included in this repository.

## Challenges and solutions
A major challenge in account abstraction is balancing flexibility with security and predictability. This repository avoids over-committing to a specific implementation up front, which keeps the codebase simple and makes it easier to evolve the smart-account design as requirements become clearer.

The solution is to build a clean, modular starting point with standard Foundry tooling and dependency management, so that more advanced account abstraction logic can be added and tested systematically.

## Setup instructions
```bash
# Install Foundry
curl -L https://foundry.paradigm.xyz | bash
foundryup

# Clone the repository
git clone https://github.com/Hayotunday/foundry-account-abstraction.git
cd foundry-account-abstraction

# Install dependencies
forge install

# Build the project
forge build

# Run tests
forge test

# Optional formatting and gas snapshot
forge fmt
forge snapshot
```

## What makes the project technically interesting
This project is interesting because account abstraction sits at the frontier of smart-wallet design. It explores how wallets can do more than simple ETH transfers by embedding programmable rules, recovery flows, and execution behavior in smart contracts. In practice, this makes it a strong learning ground for understanding how EVM accounts can evolve beyond EOAs.

## Project status
This repository is currently a Foundry-based starter and experimentation scaffold for account abstraction work. It is not yet a full production wallet implementation, but it provides the foundation for building one.

## License
The project currently follows the repository’s licensing configuration and Foundry project conventions. Check the repository files for the exact license status if needed.

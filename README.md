# protocol

> This repository hosts NFTX core contracts

## Architecture

TODO: Add architecture diagram

## Project Structure

Refer to [eth-brownie documentation](https://eth-brownie.readthedocs.io/en/stable/structure.html).

## Requirements

### Install

To run the project you need:

- Python `3.8` local development environment and Node.js `10.x` development environment for Ganache.
- Brownie local environment setup. See instructions: [ETH Brownie](https://github.com/eth-brownie/brownie).
- Local env variables for [Etherscan API](https://etherscan.io/apis) and [Infura](https://infura.io/) (`ETHERSCAN_TOKEN`, `WEB3_INFURA_PROJECT_ID`).
- Local Ganache environment installed with `npm install -g ganache-cli@6.11`.

### Run

```bash
git clone https://github.com/NFTX-project/protocol
cd protocol
yarn install --lock-file
pip install -r requirements-dev.txt
```

## Compiling Contracts

Run the following command to compile the contracts.

```
brownie compile --all
```

## Running Tests

Run tests:

```bash
brownie test -s
```

Run tests with coverage:

```bash
brownie test -s --coverage
```

## Formatting

Check linter rules for `*.json` and `*.sol` files:

```bash
yarn lint:check
```

Fix linter errors for `*.json` and `*.sol` files:

```bash
yarn lint:fix
```

Check linter rules for `*.py` files:

```bash
black . --check --config black-config.toml
```

Fix linter errors for `*.py` files:

```bash
black . --config black-config.toml
```

### Security

TODO: Add something like [this](https://github.com/iearn-finance/yearn-protocol/blob/develop/SECURITY.md)

## Documentation

You can read more about NFTX on our documentation [webpage](https://docs.nftx.org/).

### Discussion

For questions not covered in the docs, please visit [our Discord server](https://discord.gg/hytQVM5ZxR).

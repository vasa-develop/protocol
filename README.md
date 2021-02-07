# protocol

> This repository hosts NFTX core contracts

## Architecture

TODO: Add architecture diagram

## Project Structure

Refer to [eth-brownie documentation](https://eth-brownie.readthedocs.io/en/stable/structure.html).

## Requirements

### Install

- [Python3](https://www.python.org/download/releases/3.0/)
- [eth-brownie](https://eth-brownie.readthedocs.io/en/stable/install.html) **strictly `1.12.0` or above**
- Node.js 10.x development environment (for Ganache).
- Ganache (`v6.12.1` or higher)

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

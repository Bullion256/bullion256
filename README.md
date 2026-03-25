# Bullion256 (BUL)

Bullion256 is a SHA-256 proof-of-work cryptocurrency built for miners, node operators, and open-source contributors who want a fresh network with transparent rules, public infrastructure, and a straightforward launch path.

Bullion256 is designed to be simple to verify, easy to join, and friendly to real proof-of-work participation.

## Name: Bullion256
## Ticker: BUL
## Algorithm: SHA-256
## Consensus: Proof of Work
## Mining: ASIC-friendly
## Public pool: live
## Public explorer: live
## Public seed node: live
## Open-source code: public and auditable

# Why Bullion256

Bullion256 is built for people who still believe a proof-of-work network should be:

- simple to verify
- open to inspect
- easy to join
- miner friendly
- infrastructure backed from day one

This project is focused on real public participation:

- run a node
- build from source
- create a wallet
- generate an address
- connect to the network
- point your miner and start hashing

# Network Overview

- **Name:** Bullion256
- **Ticker:** BUL
- **Algorithm:** SHA-256
- **Default P2P Port:** 8368
- **Default RPC Port:** 8332

# Public Infrastructure

- **Explorer:** https://explorer.bullion256.org
- **Pool:** https://pool.bullion256.org
- **Public seed hostname:** seed.bullion256.org
- **Public seed node:** seed.bullion256.org:8368

# Stratum Mining Endpoints

- **Standard port:** `stratum+tcp://pool.bullion256.org:5555`
- **High-difficulty port:** `stratum+tcp://pool.bullion256.org:7777`

# Current Chain Direction

Bullion256 is focused on a clean, straightforward SHA-256 proof-of-work launch built for miners, node operators, and open-source contributors.

Current public direction includes:

- straightforward SHA-256 proof-of-work consensus
- ASIC-friendly mining
- public node, pool, explorer, and seed infrastructure
- transparent, auditable open-source code
- simple onboarding for miners and node operators
- compatibility-focused miner-facing proof-of-work behavior

This repository reflects the current live Bullion256 chain direction.

# Public Seed / Peer Connectivity

To help a new node join the network, add the public seed node to your config:

```conf
addnode=seed.bullion256.org:8368

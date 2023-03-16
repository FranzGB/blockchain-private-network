# Creating a private blockchain using Hyperledger Besu

This tutorial explains how to create a private blockchain using Hyperledger Besu with the QBFT (Proof of Authority) consensus protocol.

This repository will be creating a Private blockchain with 4 nodes (Because QBFT require minimum 4 nodes to operate).

In this 4 nodes one will be bootnode and others will be validators. We will be running besu from docker image for easiness.
## Requirements

- Docker
- Hyperledger Besu

## Setup

- Create a directory to store the blockchain files.
- Create a qbftConfigFile.json file inside the Private-Network/ directory and add the following code:

# Creating a private blockchain using Hyperledger Besu

This tutorial explains how to create a private blockchain using Hyperledger Besu with the QBFT (Proof of Authority) consensus protocol.

This repository will be creating a Private blockchain with 4 nodes (Because QBFT require minimum 4 nodes to operate).

In this 4 nodes one will be bootnode and others will be validators. We will be running besu from docker image for easiness.

## Requirements

- Docker
- Hyperledger Besu

## Setup

1. Change directory to `Private-Network/genesis-generator` and run `docker-compose up` to generate the block genesis file as well as the network keys.
1. Copy the block genesis file inside each of the Node folders.
1. Copy each key pair inside each of the Node folders under the `/data` directory.
1. Change directory to `Private-Network` and run `docker-compose up -d` to start the network.

You can change the `config.toml` file to change the configuration of the nodes.

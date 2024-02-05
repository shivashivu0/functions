# Token Contract 

This readme provides an overview of the `Token` smart contract, detailing its functionalities, deployment, and usage.

## Overview

The `Token` contract is an Ethereum ERC20 token implementation with additional features such as burning tokens, minting tokens (restricted to the contract owner), and checking token balances.

## Features

### ERC20 Standard Compliance

The contract adheres to the ERC20 standard, providing basic functionalities such as transfer, approve, and allowance.

### Minting Tokens

The contract owner has the exclusive right to mint new tokens. This feature can be used to increase the token supply.

### Burning Tokens

Token holders can burn their own tokens, effectively reducing the total token supply.

### Ownership

The contract is ownable, allowing for easy management and control by the designated owner.

## Deployment

To deploy the `Token` contract, follow these steps:

1. Compile the contract using a Solidity compiler compatible with version 0.8.17.
2. Deploy the compiled contract to an Ethereum network of your choice (e.g., mainnet, testnet) using a compatible Ethereum client or deployment tool.

## Usage

### Constructor Parameters

When deploying the contract, the following parameters are required:

- `_title`: A string representing the title or name of the token.
- `_code`: A string representing the symbol or code of the token.
- `starting_balance`: An unsigned integer representing the initial supply of tokens to be minted and allocated to the deployer.
- `starting_owner`: The address designated as the owner of the contract upon deployment.

### Interacting with the Contract

Once deployed, users can interact with the contract through various functions:

- `mintTokens`: Allows the contract owner to mint new tokens and allocate them to a specified address.
- `burnTokens`: Enables token holders to burn a specific amount of their own tokens, reducing the total token supply.
- `transferTokens`: Facilitates the transfer of tokens between addresses.
- `getBalance`: Retrieves the token balance of a specified address.

## License

This contract is released under the MIT License. See the SPDX-License-Identifier in the contract source code for more details.


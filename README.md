# Token Smart Contract 

## Overview

This repository contains the source code for a simple ERC-20 token smart contract named "Token." The contract is implemented in Solidity and built on the Ethereum blockchain. It includes basic functionalities such as token minting, burning, item redemption, checking player balances, and rewarding players.

## Smart Contract Features

### ERC-20 Compliance

The smart contract follows the ERC-20 standard, providing basic functionalities for managing and transferring tokens.

### Ownership

The contract extends the `Ownable` contract from OpenZeppelin, ensuring that certain functions can only be executed by the owner of the contract.

### Burning Tokens

The contract includes the ability to burn tokens, reducing the total supply.

### Item Redemption

Players can redeem items by providing a specific bounty type. Each bounty type corresponds to a different cost, and upon redemption, the player's account is debited with the appropriate amount of tokens.

### Rewarding Players

The owner of the contract can reward players by transferring tokens to their accounts. This is useful for in-game rewards or other incentivization mechanisms.

### Enumerated Bounty Types

Bounty types are represented as an enumeration (`BountyType`), with each type corresponding to a different in-game item. The cost of redeeming items is determined by the bounty type.

## Functions

- `mintTokens`: Only the owner can mint additional tokens and allocate them to a specified address.
- `burnTokens`: Only the owner can burn tokens, reducing the total supply.
- `redeemItem`: Players can redeem in-game items by specifying the bounty type, and the corresponding cost is deducted from their balance.
- `checkPlayerBalance`: Players can check their token balance.
- `rewardPlayer`: Only the owner can reward players by transferring tokens to their accounts.

## Bounty Types

The contract defines three bounty types, each representing a different in-game item:

1. Smartphone Model 1 - Cost: 200 Tokens
2. Smartphone Model 2 - Cost: 400 Tokens
3. Smartphone Model 3 - Cost: 800 Tokens

## Usage

To use the smart contract, deploy it to the Ethereum blockchain and interact with it using a blockchain wallet or through decentralized applications (DApps) that support ERC-20 tokens.

## License

This smart contract is released under the MIT License. See the `LICENSE` file for more details.

## Author

Varun

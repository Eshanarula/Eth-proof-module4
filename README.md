# DegenToken Smart Contract

## Introduction
The DegenToken is a basic ERC-20 compatible smart contract that represents a decentralized token called "Degen" (with the symbol "DGN"). This contract allows users to perform token transfers and approvals within the Ethereum blockchain.

## Contract Details
* License: MIT License
* Solidity Version: 0.8.x

## Token Information
* Name: Degen
* Symbol: DGN
* Decimals: 18
* This means that the token supports up to 18 decimal places, similar to most ERC-20 tokens. For example, if you have 1 DGN token, it would be represented as 1 * 10^18.

## Total Supply
The total supply of Degen tokens is set during the contract deployment and remains fixed.

## Functions
### Constructor
The constructor of the contract initializes the total supply of Degen tokens and assigns the entire supply to the contract deployer's address.

### transfer
This function allows token holders to transfer a specified amount of Degen tokens to another address.

### approve
This function allows token holders to approve another address (a spender) to spend a certain number of tokens on their behalf.

### transferFrom
This function is used for transferring tokens from one address to another, but it requires the approval of the sender to spend tokens on behalf of the owner.

## Events
The contract emits two events to facilitate tracking of token transfers and approvals:

* Transfer: This event is emitted whenever tokens are transferred between addresses.
* Approval: This event is emitted whenever the approval for spending tokens is granted by the token holder.

### Usage
To use the DegenToken contract, you need to deploy it on the Ethereum blockchain with an initial supply. After deployment, the contract owner will possess the total supply of Degen tokens. From there, users can perform the following actions:

* Transfer Degen tokens to other addresses using the transfer function.
* Approve other addresses to spend Degen tokens on their behalf using the approve function.
* Transfer Degen tokens on behalf of another address, given the approval, using the transferFrom function.
Please note that the contract adheres to the ERC-20 standard and can be interacted with using various Ethereum wallet applications, smart contract explorers, or other decentralized applications that support ERC-20 tokens.

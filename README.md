# Item Redeem Token (DEGEN)

## Overview

The Item Redeem Token, with the symbol DEGEN (DGN), is a Solidity smart contract built on the Ethereum blockchain. It extends the ERC-20 standard, incorporating additional features to facilitate the redemption of tokens for various snacks. The contract is equipped with the ability to mint and burn tokens, manage snack-related functionalities, and is owned by a specified address.

## Features

### ERC-20 Standard

The contract adheres to the ERC-20 token standard, providing basic functionalities like transfer, balance inquiry, and approval mechanisms.

### Token Minting and Burning

The contract owner can mint new tokens and burn existing ones. Minting is the process of creating new tokens, while burning removes tokens from circulation. These actions are restricted to the contract owner for control and security purposes.

### Snack Redemption

Users can redeem their tokens for snacks by calling the `redeemSnack` function. Each snack has a specified cost in tokens, and the contract ensures that users have sufficient funds before processing the redemption. The contract maintains a record of redeemed snacks for each user.

### Snack Management

The contract owner has the ability to modify the token cost of snacks using the `modifySnackTokenCost` function. Additionally, the owner can distribute snacks to multiple addresses using the `distributeSnacks` function.

## Snack Structure

Snacks are defined by the `Snack` struct, containing the snack name and its associated token cost. The contract initializes with a predefined set of snacks, including Pizza, Burger, Sandwich, and Milkshake.

## Events

The contract emits a `LogMessage` event during certain actions, providing transparency and allowing external systems to monitor contract activities.

## Usage

### Deployment

Deploy the contract on the Ethereum blockchain, specifying the contract owner's address.

### Minting

The contract owner can mint new tokens using the `mint` function, providing the recipient's address and the desired token amount.

### Burning

Tokens can be burned by calling the `burn` function, allowing users to reduce their token holdings.

### Snack Redemption

Users can redeem snacks by calling the `redeemSnack` function with the desired snack name as an argument. The associated token cost will be deducted from the user's balance.

### Snack Management

The contract owner can modify the token cost of snacks using the `modifySnackTokenCost` function. Additionally, snacks can be distributed to multiple addresses using the `distributeSnacks` function.

## Author

Y S Balaji 

ysbalaji4@gmail.com

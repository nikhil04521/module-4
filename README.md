# Material Token (Degen)

## Overview

Material Token, also known as Degen (DGN), is a Solidity smart contract built on the Ethereum blockchain. It extends the ERC-20 standard, providing a basic implementation of a fungible token with additional functionalities such as burning tokens, minting new tokens, redeeming jackets, and transferring jackets between addresses.

## Contract Details

- **Name:** Material Token (Degen)
- **Symbol:** DGN
- **Contract Address:** [Insert Contract Address on Ethereum Mainnet]
- **License:** MIT

## Features

1. **Minting Tokens:**
   - The contract owner can mint new tokens and send them to a specified address.

   ```solidity
   function mint(address to, uint256 tally) external onlyOwner;
   ```

2. **Burning Tokens:**
   - Token holders can burn a specific amount of their tokens, reducing the total supply.

   ```solidity
   function burn(uint256 tally) external;
   ```

3. **Redeeming Jackets:**
   - Users can redeem jackets by providing a jacket number. The contract supports jackets from Adidas, Nike, and Puma.

   ```solidity
   function redeemJacket(uint8 jacketNumber) external;
   ```

4. **Transferring Jackets:**
   - Users can transfer jackets (tokens) to other addresses.

   ```solidity
   function transferJackets(address recipient, uint256 tally) external;
   ```

## Jacket Types

The contract defines three types of jackets:
- Adidas
- Nike
- Puma

Each jacket type has an associated cost in the contract.

## Usage

1. **Deployment:**
   - Deploy the contract on the Ethereum blockchain.
   - Specify the initial owner's address during deployment.

2. **Initialization:**
   - The contract initializes with predefined costs for each jacket type.

3. **Minting:**
   - The owner can mint new tokens to a specified address.

4. **Burning:**
   - Token holders can burn a specific amount of their tokens.

5. **Redeeming Jackets:**
   - Users can redeem jackets by providing a jacket number and burning the required tokens.

6. **Transferring Jackets:**
   - Users can transfer jackets (tokens) to other addresses.

## License

This contract is licensed under the MIT License. See the `LICENSE` file for details.

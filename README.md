# MyToken Contract

## Overview
MyToken is a Solidity smart contract that implements a basic ERC20 token with additional functionalities such as activation, minting, burning, transferring tokens, and managing token transfer permissions. It allows the creator to activate the token, mint new tokens, burn tokens, transfer tokens, and control token transfer permissions.

## Features
- **ERC20 Token**: Implements the ERC20 standard for fungible tokens.
- **Activation**: Allows the creator to activate the token, enabling transfers.
- **Minting**: Allows the creator to mint new tokens and distribute them to designated addresses.
- **Burning**: Enables token holders to burn their tokens, reducing the total supply.
- **Transferring**: Facilitates the transfer of tokens between addresses.
- **Transfer Permission Control**: Allows the creator to disable token transfers.

## Contract Structure
- **ERC20**: Inherits from OpenZeppelin's ERC20 contract to implement the basic token functionalities.

## Functions
- `activateToken`: Activates the token, allowing transfers and mints initial tokens to the creator's address.
- `mintTokens`: Allows the creator to mint new tokens and assign them to a specified address.
- `burnTokens`: Allows token holders to burn a certain amount of their tokens.
- `transferTokens`: Enables token holders to transfer tokens to another address.
- `getAccountBalance`: Retrieves the token balance of the specified account.
- `disableTransfer`: Allows the creator to disable token transfers.

## Usage
1. Deploy the contract to the Ethereum blockchain.
2. Activate the token using `activateToken` function.
3. Mint initial tokens to designated addresses using `mintTokens` function.
4. Users can interact with the contract to burn, transfer, and query token balances.
5. The creator can disable token transfers using `disableTransfer` function.

## Security Considerations
- Ensure proper access control to critical functions.
- Validate user inputs to prevent potential vulnerabilities.
- Implement proper error handling and revert conditions.

## Disclaimer
This contract is provided as-is for demonstration purposes only. Use it at your own risk and ensure proper auditing and testing before deploying it in a production environment.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

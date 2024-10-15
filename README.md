# Implementing_an_ERC20_Token

**Overview-**
This project provides an implementation of the ERC-20 token standard. It includes the basic functionality required for creating and managing a fungible token on the Ethereum blockchain, as defined by the EIP-20 Token Standard (https://eips.ethereum.org/EIPS/eip-20).

**Features-**

- ERC-20 Standard Compliant: Implements standard functions and events for interoperability with wallets, exchanges, and other services.
- Core Functionalities:
  - totalSupply: Returns the total number of tokens in existence.
  - balanceOf: Provides the token balance of a given address.
  - transfer: Allows token holders to transfer their tokens to another address.
- Allowance Mechanism:
  - approve: Approves a specified address to spend a certain number of tokens on behalf of the token owner.
  - transferFrom: Allows the transfer of tokens from an approved address.
  - allowance: Returns the number of tokens that a spender is still allowed to withdraw from the owner.

**Prerequisites-**

- Solidity Compiler: Version >=0.5.0 <0.9.0
- Ethereum Development Tools: Such as Truffle, Hardhat, or Remix for deployment and interaction.

**How to Deploy-**

1. Set Up Your Development Environment: Use Truffle, Hardhat, or Remix to set up a development environment.
2. Compile the Contract: Make sure to use a compatible Solidity compiler version.
3. Deploy the Contract to the Blockchain: Use your development tools to deploy the compiled contract to the desired Ethereum network.

**Usage Examples-**

Basic Token Operations

- Check Total Supply:
  uint256 totalSupply = token.totalSupply();

- Check Balance of an Address:
  uint256 balance = token.balanceOf(address);

- Transfer Tokens to Another Address:
  bool success = token.transfer(recipientAddress, amount);

**Allowance-Based Operations-**

1. Approve a Spender:
   bool success = token.approve(spenderAddress, amount);

2. Transfer Tokens on Behalf of the Owner:
   bool success = token.transferFrom(ownerAddress, recipientAddress, amount);

**License-**

This project is licensed under the MIT License.




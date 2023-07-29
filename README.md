# Eth-avax-module3

# MyToken Smart Contract (21BCS3361)

This is a basic Ethereum ERC20-compliant token smart contract written in Solidity. The contract represents a simple token called "21BCS3361" with the symbol "Priya." The contract allows the owner to mint new tokens, burn existing tokens, and transfer tokens to other addresses.

## Contract Details

### Token Information

- **Token Name**: 21BCS3361
- **Token Symbol**: Priya
- **Total Supply**: 1,000,000

### Functions

#### Mint

The `mint` function allows the contract owner to mint new tokens and assign them to a specific address.

```solidity
function mint(address to, uint256 amount) external onlyOwner
```

Parameters:
- `to`: The address to which the newly minted tokens will be assigned.
- `amount`: The number of tokens to mint and assign to the given address.

#### Burn

The `burn` function enables any address to burn their existing tokens, thereby reducing the total supply.

```solidity
function burn(uint256 amount) external
```

Parameters:
- `amount`: The number of tokens to burn from the sender's address.

#### Transfer

The `transfer` function allows any address to transfer their tokens to another address.

```solidity
function transfer(address to, uint256 amount) external
```

Parameters:
- `to`: The address to which the tokens will be transferred.
- `amount`: The number of tokens to transfer to the given address.

### Ownership and Access Control

The contract includes a modifier `onlyOwner` to restrict certain functions to be callable only by the contract owner.

## How to Use

1. Deploy the smart contract to an Ethereum blockchain (e.g., using Remix, Truffle, or other development tools).
2. After deployment, you will get the contract address.
3. The contract creator is the initial owner of all tokens.
4. Use the `mint` function with the contract owner's address to mint new tokens and distribute them to specific addresses.
5. Use the `burn` function to burn tokens from any address, effectively reducing the total supply.
6. Use the `transfer` function to transfer tokens between addresses.

## License

This smart contract is released under the MIT License. You can find the license text in the SPDX-License-Identifier comment in the contract code.


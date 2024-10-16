# MyToken Smart Contract

A basic smart contract implementation for creating a custom token with mint and burn functionalities using Solidity.

## Description

The MyToken contract is a simple example of an ERC-20-like token implemented in Solidity. It allows the creation of a token with a name, abbreviation, and total supply. 
The contract supports minting new tokens to specified addresses and burning tokens, reducing the total supply. It includes essential checks to ensure users cannot burn 
more tokens than they own.

## Getting Started

### Installing

1. Download the project:
* You can copy the Solidity code and paste it into any Solidity-compatible IDE, such as Remix.
* Alternatively, if you are working with a local setup, download the project and place it in your Solidity workspace.

2. Set up a development environment:
* You need to have the Solidity compiler (solc) installed.
* Make sure to use Solidity version 0.8.18 or a compatible version.
  
3. Modifications:
* You can modify the token name, abbreviation, or any other details by adjusting the public variables within the contract.

### Executing program

1. Deploy the contract:
* Compile the smart contract using a Solidity IDE or your local compiler.
* Deploy the contract on a test blockchain (like Ganache or a test network).

2. Mint tokens:
* Call the mint function to increase the total supply and add balance to an address.
solidity
```
mint(0xYourAddress, 1000);
```
This will mint 1000 tokens to 0xYourAddress and increase the total supply by 1000.

3. Burn tokens:
* Call the burn function to reduce the total supply and remove tokens from an address.
solidity
```
burn(0xYourAddress, 500);
```
This will burn 500 tokens from 0xYourAddress and reduce the total supply accordingly.


## Help

Common issues:
* Insufficient balance: When trying to burn tokens, ensure that the address has enough balance to burn. 
The burn function will execute but will fail to change the balance if the balance is less than the burn amount.
* Correct contract version: Ensure you are using the Solidity compiler version 0.8.18 to avoid compatibility issues.
  
If your program contains helper functions or error-handling mechanisms, you can check the documentation within the IDE for more information.

## Authors

Daniel Jude Seno - Contact via [GitHub](https://github.com/djrseno)

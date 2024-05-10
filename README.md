# Solidity Functions and Error Handling

Overview

This Ethereum smart contract, coded in Solidity, facilitates withdrawals, deposits, and balance checks for users. It showcases the implementation of require(), revert(), and assert() statements for managing errors and validating inputs.

## Prerequisites
To interact with the smart contract, you'll require:
* A development environment for Ethereum smart contracts.
* An Ethereum wallet or client (e.g., MetaMask) for compiling, deploying, and interacting with the smart contract.

## How to Use
1. Deploy the smart contract on a compatible Ethereum Virtual Machine (EVM), utilizing Solidity compiler version 0.8.25 or higher.
2. Engage with the contract via transactions, invoking the deposit and withdraw functions with appropriate parameters.
3. Ensure smooth exception handling, comprehending the error messages returned by require(), assert(), and revert() statements.

## Details of the Smart Contract
The smart contract, MyContract, encompasses the following functions:

### deposit(address _address, uint _value)
This function enables users to deposit funds into their accounts. It validates whether the deposit value exceeds 100 using the require() statement. Subsequently, funds are added to the user's balance. Following this, the assert() statement confirms that the balance has genuinely increased by the deposited amount. If not, the transaction is reverted with an error message.

### withdraw(address _address, uint _value)
Users can withdraw funds from their accounts via this function. It ensures the user possesses adequate balance through require(). Upon successful validation, the specified amount is deducted from the user's balance. Analogous to the deposit function, the assert() statement verifies that the balance remains non-negative post-withdrawal. If it fails, the transaction is reverted with a relevant error message.

## Author
Sean Ydnar A. Abellanosa

## License
This project operates under the MIT License - refer to the LICENSE.md file for specifics.


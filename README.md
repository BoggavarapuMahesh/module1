# module1
Project Title: Handling Smart Contract

Description:
This Solidity smart contract demonstrates handling techniques using the `assert()`, `revert()`, and `require()` statements. It includes functions to test the `assert()` statement, perform division with error checking, and execute multiplication with a `require()` condition.

Prerequisites
Solidity ^0.8.17 

License
This contract is using the MIT License.

Executing Program:
After compiling the smart contract, you can deploy it to a local or testnet Ethereum network using your development environment. Once deployed, you can interact with the contract through the deployed instance.

To execute the program, follow these steps:

1. Deploy the smart contract to an Ethereum network using your Solidity development environment.

2. Once deployed, you can call the `testAssert`, `divide`, and `mult` functions.

3. The `testAssert` function takes an input parameter `num` and executes an `assert()` statement. If `num` is equal to zero, the assertion fails, and the transaction reverts.

4. The `divide` function performs a division operation with error checking. It takes two input parameters `_numerator` and `_denominator`. If `_numerator` is less than `_denominator`, the function reverts with a custom error message.

5. The `mult` function performs multiplication of an input parameter `a` with a predefined variable `b`. It includes a `require()` statement to ensure that `a` is greater than zero. If `a` is zero, the function reverts with a custom error message.

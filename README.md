# TestError Contract

This contract implements a simple driving test scenario with error handling functionalities. It allows users to perform the following actions:

- Determine the number of years until a person becomes an adult.
- Check if a person is eligible to drive and provide a message accordingly.
- Set the number of driving test attempts.

## Contract Details

- SPDX-License-Identifier: MIT
- Solidity Version: ^0.8.17

## Functions

### minor

solidity
function minor(uint _age) public pure returns(uint)


This function takes an `_age` parameter and returns the number of years remaining until the person becomes an adult (18 years old). If the provided age is greater than 18, the function reverts with an error message: "Person is already an adult."

### drive

solidity
function drive(uint _age) public pure returns(string memory)


The `drive` function takes an `_age` parameter and returns a message indicating whether the person is eligible to drive. If the age is less than 18, the function reverts with an error message: "You are not eligible to drive." Otherwise, it returns the message "Have fun driving."

### trial

solidity
function trial(uint attempts) public


This function sets the number of driving test attempts by updating the `drivingTestTrial` variable. It takes an `attempts` parameter and assigns its value to `drivingTestTrial`. Additionally, it uses an `assert` function to ensure that the `drivingTestTrial` value is greater than zero.

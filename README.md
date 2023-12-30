# Zoo Entry VIP 

## Overview

This Solidity smart contract, named `ZooEntryVIP`, manages access to a VIP zone in a zoo based on the age of individuals. It is designed to restrict entry to those within a specified age range and with additional conditions.

## Features

- **Age Restrictions:** The contract sets a minimum and maximum age limit for VIP entry, defined as `minAge` and `maxAge` respectively.

- **Event Emission:** The contract emits an event `AllowedVIPEntry` when a user successfully enters the VIP zone. The event includes the address of the entrant and their age.

- **Entrance Conditions:** The `enterVIPZone` function allows individuals to enter the VIP zone by providing their age. It checks whether the age is within the specified range and emits the `AllowedVIPEntry` event if the conditions are met.

- **Additional Condition:** There is an extra condition using the `revert` statement that restricts entry to individuals with even ages. If an individual's age is not even, the function reverts with a corresponding error message.

- **Internal Consistency Check:** The contract includes an `assert` statement to ensure that the age provided is non-negative. This acts as an internal consistency check.

## Usage

1. **Deploy the Contract:** Deploy the `ZooEntryVIP` contract to the Ethereum blockchain.

2. **Enter VIP Zone:** Users can call the `enterVIPZone` function, providing their age as an argument. If the age is within the specified range and satisfies the additional condition, the user is granted VIP entry, and the `AllowedVIPEntry` event is emitted.

## License

This smart contract is released under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author 
Kantesh
kanteshmh11@gmail.com

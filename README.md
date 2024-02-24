# Function-Frontend


### Overview
This repository contains a simple React component for a dapp. Users can connect their MetaMask wallet, view their account balance, deposit and withdraw ETH, and check the owner's name. The application interacts with a Solidity smart contract deployed on the Ethereum blockchain.

### Smart Contract - 
The  smart contract serves as the core component of the Crypto ATM application. It provides the following functionalities:

#### `getBalance()`
Returns the current balance of the contract.

#### `deposit(uint256 _amount)`
Allows users to deposit the specified amount of funds into the contract.

### Frontend Integration
The functions from the `Assessment.sol` smart contract are integrated into the frontend of the application to provide a seamless user experience:

- The `getBalance()` function fetches and displays the current balance of the contract on the user interface.
- The `deposit(_amount)` function is invoked when users want to deposit funds into the contract. They can enter the amount they wish to deposit, and the frontend handles the transaction and updates the balance accordingly.

### Commands
To get the code running on your computer, follow these steps:

1. Inside the project directory, run `npm install` to install dependencies.
2. Open two additional terminals in your VS code.
3. In the second terminal, run `npx hardhat node` to start the local Ethereum node.
4. In the third terminal, run `npx hardhat run --network localhost deploy/deploy.js` to deploy the smart contract.
5. Back in the first terminal, run `npm run dev` to launch the front-end.

### License
This project is licensed under the MIT License. See the LICENSE file for details.

### Disclaimer
- This application is intended for educational purposes only and should not be used in a production environment without proper testing and security audits.
- Users are responsible for any risks associated with interacting with the Ethereum blockchain and smart contracts.

--- 

Feel free to customize this README according to your project's requirements, providing additional details or instructions as needed.

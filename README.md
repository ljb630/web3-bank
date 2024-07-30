# Web3 Bank

A simple Web3 bank application built with React and Ethereum smart contracts. This project demonstrates basic functionalities of a blockchain-based bank, allowing users to deposit and withdraw Ether using a smart contract.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup](#setup)
- [Usage](#usage)
- [Smart Contract Deployment](#smart-contract-deployment)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Connect with MetaMask:** Uses MetaMask or another Ethereum wallet provider for account management.
- **Deposit Ether:** Allows users to deposit Ether into the smart contract.
- **Withdraw Ether:** Enables users to withdraw Ether from the smart contract.
- **View Balance:** Displays the current balance in the smart contract.

## Tech Stack

- **Frontend:** React, Web3.js
- **Blockchain:** Ethereum
- **Smart Contracts:** Solidity
- **Development Environment:** Ganache (for local blockchain simulation)

## Setup

### Prerequisites

- **Node.js**: [Install Node.js](https://nodejs.org/)
- **npm or yarn**: [npm](https://www.npmjs.com/) or [yarn](https://classic.yarnpkg.com/)

### Installation

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/ljb630/web3-bank.git
    ```

2. **Navigate to the Project Directory:**

    ```bash
    cd web3-bank/web3-bank-frontend
    ```

3. **Install Dependencies:**

    ```bash
    npm install
    # or
    yarn install
    ```

4. **Compile and Migrate Smart Contracts:**

    Follow the instructions in the `web3-bank/web3-bank-smart-contract` directory to compile and migrate your smart contracts using Truffle or Hardhat.

5. **Start the Frontend Application:**

    ```bash
    npm start
    # or
    yarn start
    ```

    The application will run on [http://localhost:3000](http://localhost:3000).

## Usage

1. **Connect Wallet:** Ensure you have MetaMask installed and connected to your local blockchain (e.g., Ganache).
2. **Deposit Ether:** Enter the amount of Ether you want to deposit and click the "Deposit" button.
3. **Withdraw Ether:** Enter the amount of Ether you want to withdraw and click the "Withdraw" button.
4. **View Balance:** Your balance will be displayed on the frontend.

## Smart Contract Deployment

To deploy the smart contract:

1. **Navigate to the `web3-bank-smart-contract` Directory:**

    ```bash
    cd web3-bank/web3-bank-smart-contract
    ```

2. **Compile Contracts:**

    ```bash
    truffle compile
    ```

3. **Migrate Contracts:**

    ```bash
    truffle migrate
    ```

4. **Update Frontend with Contract Details:**

    Update the `Bank.json` file in the `web3-bank/web3-bank-frontend/src/contracts` directory with the contract ABI and address from the deployment.

## Troubleshooting

- **Failed to Fetch Error:** Ensure your Ethereum node or Ganache is running and accessible. Verify the network configuration in your application.
- **Contract Not Deployed Error:** Check that the smart contract is correctly deployed to the network and that the ABI and address in `Bank.json` are correct.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adjust and expand upon this template based on the specifics of your project.


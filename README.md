# STKN ICO DApp (Decentralized ICO Application)

```markdown
# STKN ICO DApp (Decentralized ICO Application)

Welcome to the STKN ICO DApp, a decentralized web3 application that allows users to participate in an Initial Coin Offering (ICO) and purchase newly created **STKN** (ERC20) tokens. The application is built on blockchain technology, ensuring a secure and trustless environment. This project is composed of two main parts:

- **Client**: The frontend web interface for users to interact with the ICO.
- **Smart Contract**: The backend logic deployed on the Ethereum Goerli TestNet to manage the ICO process and token distribution.

## Features

- **Decentralized Token Sale**: Users can buy STKN tokens directly from the DApp.
- **ERC20 Token**: The STKN token follows the ERC20 standard for compatibility and ease of integration.
- **Blockchain-Powered**: The app operates on the Goerli TestNet to provide decentralized and trustless transactions.
- **Secure & Transparent**: All ICO transactions are managed via smart contracts, ensuring security and transparency.

## Project Structure
```
root/
│
├── client/
│   ├── src/
│   ├── public/
│   └── package.json
│
└── smart-contract/
    ├── contracts/
    ├── scripts/
    └── hardhat.config.js
```

### 1. **Client** (Frontend)

The client folder contains the user interface code, built using React.js and Web3.js to connect to the blockchain and interact with the smart contract.

### 2. **Smart Contract** (Backend)

The smart-contract folder contains the Ethereum smart contract code, written in Solidity. This folder uses the Hardhat framework for contract development, deployment, and testing.

---

## Installation and Setup

### Prerequisites

Ensure you have the following installed before getting started:

- **Node.js**: [Download Node.js](https://nodejs.org/)
- **MetaMask**: [MetaMask Wallet](https://metamask.io/) extension for connecting your wallet.
- **Hardhat**: For smart contract deployment and testing.

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/stkn-ico-dapp.git
cd stkn-ico-dapp
```

### 2. Smart Contract Setup

Navigate to the `smart-contract` folder to install dependencies and deploy the contract:

```bash
cd smart-contract
npm install
```

#### Deploy Smart Contract

To deploy the smart contract to the Goerli TestNet, you need to set up environment variables:

1. Create a `.env` file in the `smart-contract` directory with the following contents:

```plaintext
GOERLI_URL="https://goerli.infura.io/v3/YOUR_INFURA_PROJECT_ID"
PRIVATE_KEY="YOUR_METAMASK_PRIVATE_KEY"
```

2. Compile and deploy the contract:

```bash
npx hardhat compile
npx hardhat run scripts/deploy.js --network goerli
```

### 3. Client Setup

Next, move to the `client` folder to set up the frontend:

```bash
cd ../client
npm install
```

Create a `.env` file in the `client` directory with your contract address and Infura details:

```plaintext
REACT_APP_CONTRACT_ADDRESS="YOUR_DEPLOYED_CONTRACT_ADDRESS"
REACT_APP_INFURA_URL="https://goerli.infura.io/v3/YOUR_INFURA_PROJECT_ID"
```

#### Run the Client

```bash
npm start
```

This will start the React development server. Open [http://localhost:3000](http://localhost:3000) in your browser to access the DApp.

---

## Usage

### User Flow

1. **Connect Wallet**: Users can connect their Ethereum wallet (e.g., MetaMask) via the “Connect Wallet” button.
2. **Buy STKN Tokens**: After connecting the wallet, users can enter the amount of ETH they want to spend to purchase STKN tokens.
3. **Confirm Transaction**: The app will prompt users to confirm the transaction in MetaMask, and the smart contract will handle the token purchase.
4. **Check Balance**: Users can check their STKN token balance after the transaction is completed.

---

## Smart Contract Details

- **Token Name**: STKN Token
- **Token Symbol**: STKN
- **Token Standard**: ERC20
- **Network**: Goerli TestNet

The smart contract is responsible for handling token sales, minting new tokens for purchasers, and managing ICO stages.

---

## Testing

### Smart Contract Tests

You can run tests for the smart contract using Hardhat. To execute tests, run the following command inside the `smart-contract` folder:

```bash
npx hardhat test
```

### Frontend Tests

To run tests for the client-side React app, use:

```bash
npm test
```

---

## Technologies Used

- **Solidity**: For writing the smart contract.
- **React.js**: Frontend library for building the user interface.
- **Hardhat**: Development environment for Ethereum smart contracts.
- **Web3.js**: Ethereum JavaScript API to interact with the blockchain.
- **MetaMask**: Wallet extension to connect to Ethereum.

---

## License

This project is licensed under the MIT License.

---
## 🚀 Contact

For any questions, feedback, or inquiries, feel free to reach out to **Mohsin Ali Solangi**. You can connect via the following platforms:

🌐 **Linktree**: [Mohsin Ali Solangi](https://linktr.ee/mohsinalisolangi)

🔗 **LinkedIn**: [Mohsin Ali Solangi](https://www.linkedin.com/in/mohsinalisolangi/)

Looking forward to hearing from you! 😄

### Key Sections:
1. **Features**: Highlights the key functionality of the app.
2. **Project Structure**: Provides an overview of the folder structure for better understanding.
3. **Installation & Setup**: Step-by-step instructions to get the app running.
4. **Smart Contract & Client**: Divides focus between frontend and backend setup.
5. **Usage**: Shows how users will interact with the DApp.
6. **Testing**: Explains how to test both the smart contract and frontend.
7. **Technologies Used**: Lists the tech stack to demonstrate the tools and frameworks involved.

```



# DigitalWill: A Decentralized Application for Digital Inheritance

DigitalWill is a blockchain-based decentralized application (dApp) that allows users to create and manage their last will and testament in a secure and transparent manner. By leveraging smart contracts on the Ethereum blockchain, DigitalWill ensures that your digital assets are distributed to your designated beneficiaries according to your wishes, without the need for traditional intermediaries.

This project provides a user-friendly interface for creating a digital will, specifying assets (both fungible ERC20 tokens and non-fungible ERC721 tokens/NFTs), and appointing an executor to carry out the will's instructions.

## Key Features

*   **Decentralized Will Creation:** Create a legally binding digital will on the Ethereum blockchain.
*   **Asset Management:** Include various digital assets in your will, such as cryptocurrencies (ERC20 tokens) and unique digital collectibles (ERC721 NFTs).
*   **Beneficiary Designation:** Clearly specify the beneficiaries for each of your assets.
*   **Executor Appointment:** Appoint a trusted individual as the executor of your will.
*   **Secure Execution:** The will can only be executed by the designated executor, ensuring your assets are distributed as intended.
*   **Transparency and Immutability:** All will data is stored on the blockchain, providing a transparent and tamper-proof record of your final wishes.

## Technologies Used

*   **Solidity:** The smart contract is written in Solidity, the primary programming language for Ethereum.
*   **OpenZeppelin Contracts:** Utilizes the secure and battle-tested OpenZeppelin library for ERC20 and ERC721 token standards.
*   **Ethers.js:** A complete and compact library for interacting with the Ethereum Blockchain and its ecosystem.
*   **MetaMask:** A crypto wallet and gateway to blockchain apps, used for connecting to the dApp and signing transactions.
*   **HTML, CSS, and JavaScript:** The frontend of the application is built using standard web technologies.

## How it Works

The DigitalWill dApp consists of a smart contract deployed on the Ethereum blockchain and a web-based user interface.

### Smart Contract (`DigitalWill.sol`)

The core logic of the application resides in the `DigitalWill.sol` smart contract. This contract allows users to:

1.  **Create a Will:** A new will is created with the user's name, date of birth, an appointed executor, and a list of assets to be distributed.
2.  **Update a Will:** The creator of a will can update the list of assets at any time before the will is executed.
3.  **Execute a Will:** The designated executor can trigger the execution of the will, which transfers the specified assets to the beneficiaries.

### Frontend (`index.html`, `main.js`, `styles.css`)

The frontend provides a user-friendly interface for interacting with the smart contract. Users can:

1.  **Connect their MetaMask Wallet:** Connect to the dApp using their MetaMask wallet.
2.  **View Will Details:** See the total number of wills created on the platform.
3.  **Create a New Will:** Fill out a form to create a new digital will, specifying their personal details, executor, and assets.

## Getting Started

To run this project locally, you will need to have Node.js and a package manager like npm or yarn installed.

### Prerequisites

*   Node.js
*   npm or yarn
*   MetaMask browser extension

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Alhibb/DigitalWill.git
    ```
2.  **Install the dependencies:**
    ```bash
    cd DigitalWill
    npm install
    ```
3.  **Compile the smart contract:**
    You will need a development environment like Hardhat or Truffle to compile the `DigitalWill.sol` contract.
4.  **Deploy the smart contract:**
    Deploy the compiled contract to a local or public test network (e.g., Ropsten, Rinkeby, or a local Ganache instance).
5.  **Update the contract address:**
    In `main.js`, replace the placeholder `contractAddress` with the actual address of your deployed smart contract.
6.  **Run the application:**
    Open the `index.html` file in your browser.

## Usage

1.  Open the application in your browser.
2.  Click the "Connect MetaMask Wallet" button to connect your wallet.
3.  Once connected, you will see the total number of wills created.
4.  Fill out the "Create New Will" form with your personal details, the executor's address, and the assets you wish to include.
5.  Click "Create Will" and confirm the transaction in MetaMask.

## Disclaimer

This project is for educational purposes only and should not be used for creating legally binding wills without consulting with a legal professional. The security of the smart contract has not been professionally audited. Use at your own risk.

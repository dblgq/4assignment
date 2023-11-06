# Project Setup Guide

Welcome to the project! This guide will walk you through the steps to get the project running on your machine.

## How to Install and Run the Project

Before diving into the code, let's set up the environment:

### Prerequisites
- Node.js installed on your machine.
- Access to a terminal or command-line interface.

### Installation

1. Clone the repository to your local machine.
2. Navigate to the project directory in your terminal.
3. Install all the necessary dependencies by running the following command:
   ```zsh
   npm install
   ```
4. Create a `.env` file in the root of the project and paste the following lines with your respective values:
   - `NETWORK` - The blockchain network you are using.
   - `INFURA_URL` - Your Infura URL, which looks like `https://sepolia.infura.io/v3/YOUR-API-KEY`.
   - `PRIVATE_KEY` - The private key of your MetaMask account.
   - `ETHERSCAN_API` - The API key from etherscan.io.
   - `OWNER` - Your wallet address, for example, `0xd3106F16102e2AEF6AC5D3E371c121885aa4f82e`.

### Compilation

To compile the smart contract, use the command:
```zsh
make compile
```

### Deployment

Deploy your contract to the network with:
```zsh
make deploy
```

### Verification

Verify the contract by providing the contract's address as follows:
```zsh
make address=*your_contract_address* verify
```

### Running the Server

To run a local development server:
```zsh
make run
```

### Testing

Execute tests using:
```zsh
make ctest
```

## React Application

This project includes a frontend built with Create React App.

### Development Server

To start the app in development mode, run:
```zsh
npm start
```
Your default web browser will open [http://localhost:3000](http://localhost:3000) automatically.

### Running Tests

Interactive tests can be conducted with:
```zsh
npm test
```

### Building for Production

To create a production build, use:
```zsh
npm run build
```
This compiles the app and optimizes the build for performance.

### Customization

If you need to eject from the Create React App defaults (not recommended), you can do so using:
```zsh
npm run eject
```
**Warning:** This action is irreversible.

## Additional Information

For more details, refer to the Create React App documentation and learn about React through the official React documentation.

By following these steps, you should have a fully functional local development environment for both the smart contract and the React application. Happy coding!
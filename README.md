# Project-Degen-Token-ERC-20-Unlocking-the-Future-of-Gaming

# DegenToken

DegenToken is an ERC20-based token system with functionality for minting, transferring, burning, and redeeming tokens for an in-game asset called "souls." The owner has exclusive rights to mint new tokens, while all users can transfer, check balances, redeem for souls, and burn their tokens.

## Description

DegenToken is a smart contract built on the Ethereum blockchain using Solidity. This contract implements a token with the following functionalities:
- Minting new tokens (only accessible by the contract owner)
- Transferring tokens between players
- Redeeming tokens for in-game items (souls)
- Checking token balances
- Burning tokens that are no longer needed

This project can be used in any blockchain-based game or application that requires an ERC20 token with the above features.

## Getting Started

### Installing

1. Clone the repository from GitHub:
    ```bash
    git clone https://github.com/your-repo/DegenToken.git
    ```
2. Navigate to the project directory:
    ```bash
    cd DegenToken
    ```
3. Install the necessary dependencies (assuming you are using Node.js and npm):
    ```bash
    npm install
    ```

### Executing program

To deploy and interact with the DegenToken contract, follow these steps:

1. Compile the contract:
    ```bash
    npx hardhat compile
    ```
2. Deploy the contract to a local blockchain (e.g., Hardhat Network):
    ```bash
    npx hardhat run scripts/deploy.js --network localhost
    ```
3. Interact with the contract using Hardhat console or a front-end application.

Example commands to interact with the contract:
```javascript
// Minting tokens (onlyOwner)
await degenToken.mintTokens("0xAddress", 1000);

// Transferring tokens
await degenToken.transferTokens("0xRecipientAddress", 100);

// Redeeming souls
await degenToken.redeemSoul(5);

// Checking token balance
let balance = await degenToken.checkBalance("0xAddress");
console.log(balance.toString());

// Burning tokens
await degenToken.burnTokens(50);
```


## HELP:
```bash
npx hardhat help
```

## AUTHOR
itstudent2021

## License

License - see the `LICENSE.md` file for details


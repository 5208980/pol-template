# Creating and Deploying an ERC20 Token with OpenZeppelin

Welcome! In this tutorial, we'll explore how to create and deploy your very own ERC20 token using OpenZeppelin's library. ERC20 tokens are the standard for fungible tokens on the Ethereum blockchain, meaning each token is identical in value and function.

## What is OpenZeppelin?

OpenZeppelin is a library for secure smart contract development. It provides implementations of popular token standards, including ERC20, which you can use to create your own tokens without having to reinvent the wheel. Using OpenZeppelin's implementations ensures that your token adheres to best practices and standards in the Ethereum ecosystem.

### Example Contract: MyToken

Let's start with an example contract that creates a simple ERC20 token called MyToken with the symbol MTK.

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract MyToken is ERC20 {
    constructor() ERC20("MyToken", "MTK") {}
}
```

### Explanation

1. **Pragma Statement:** `pragma solidity ^0.8.20;` specifies the version of Solidity to be used.
2. **Import Statement:** `import "@openzeppelin/contracts/token/ERC20/ERC20.sol";` imports the ERC20 contract from OpenZeppelin's library.
3. **Contract Definition:** `contract MyToken is ERC20` declares a new contract that inherits from the ERC20 contract.
4. **Constructor:** The constructor sets the token's name to "MyToken" and the symbol to "MTK" by calling the ERC20 constructor.

By inheriting from OpenZeppelin's ERC20 contract, we automatically get all the standard functionalities of an ERC20 token, such as transferring tokens, checking balances, and approving allowances.

## Task: Create and Deploy Your Own ERC20 Token

Now, it's your turn to create and deploy your own ERC20 token! Follow these steps to create a token called TokenPoken with the symbol TP.

### Step-by-Step Guide

### Step 2: Write the Smart Contract

In `TokenPoken.sol`, write the following code:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract TokenPoken is ERC20 {
    constructor() ERC20("TokenPoken", "TP") {}
}
```

### Step 3: Compile the Contract

2. **Select the Compiler Version:** Select version 0.8.20 from the "Compiler" dropdown menu.
3. **Compile the Contract:** Click the "Compile TokenPoken.sol" button. If there are no errors, you should see a green checkmark indicating successful compilation.

### Step 4: Deploy the Contract

1. **Open the Deploy & Run Transactions Tab:** Navigate to the "Deploy & Run Transactions" tab on the left sidebar.
2. **Select the Environment:** Choose "Injected Web3" from the "Environment" dropdown menu to deploy using MetaMask.
3. **Connect MetaMask:** MetaMask will prompt you to approve the connection.
4. **Deploy the Contract:** Ensure that `TokenPoken` is selected in the "Contract" dropdown menu. Click the "Deploy" button. MetaMask will prompt you to confirm the transaction.
5. **Confirm Deployment:** Confirm the transaction in MetaMask. Once the transaction is confirmed, your contract will be deployed.

### Testing Your Token

After deploying your TokenPoken contract, you can interact with it using the functions inherited from the ERC20 contract. Here are a few things you can try:

1. **Check the Total Supply:** Call the `totalSupply` function to see the total supply of TokenPoken tokens.
2. **Check Your Balance:** Call the `balanceOf` function with your address to check your token balance.
3. **Transfer Tokens:** Use the `transfer` function to send tokens to another address.

### Conclusion

Congratulations! You've successfully created and deployed your own ERC20 token called TokenPoken with the symbol TP using OpenZeppelin's ERC20 contract. This exercise demonstrates the power and ease of using OpenZeppelin for secure and standardized smart contract development.
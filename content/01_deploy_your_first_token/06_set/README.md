# Interacting with Your Contract: Setting the Name and Retrieving the Transaction Hash

Now that your contract is deployed on the Open Campus Codex network, let's interact with it by setting the name to "Vitalik" and retrieving the transaction hash of this call. The transaction hash is a unique identifier for the transaction on the blockchain, allowing you to track and verify the transaction.

### Step-by-Step Guide to Setting the Name and Getting the Transaction Hash

### Step 9: Set the Name to "Vitalik"

2. **Find Your Deployed Contract:** Under "Deployed Contracts," expand your deployed contract to see its functions.
3. **Set the Name:** In the `setName` function input box, type `"Vitalik"` (including the quotes). Click the "transact" button to send the transaction.
4. **Confirm in MetaMask:** MetaMask will prompt you to confirm the transaction. Review the details and click "Confirm."

### Step 10: Retrieve the Transaction Hash

Once the transaction is confirmed will display the transaction details, including the transaction hash. Here’s how you can retrieve it:

1. **Transaction Receipt:** After confirming the transaction in MetaMask, will show a transaction receipt in the "Deploy & Run Transactions" tab.
2. **Copy the Transaction Hash:** Look for the field labeled "transaction hash" in the receipt. This is a unique identifier for your transaction. Copy this hash for future reference.

### Example of Setting the Name and Retrieving the Transaction Hash

Let's illustrate this process with an example. Suppose your contract looks like this:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleContract {
    string value;
    string name;

    // Getter for the 'value' variable
    function getValue() public view returns (string memory) {
        return value;
    }

    // Setter for the 'value' variable
    function setValue(string memory _value) public {
        value = _value;
    }

    // Getter for the 'name' variable
    function getName() public view returns (string memory) {
        return name;
    }

    // Setter for the 'name' variable
    function setName(string memory _name) public {
        name = _name;
    }
}
```

After deploying this contract, follow the steps above to set the name to "Vitalik" and get the transaction hash.

### What Just Happened?

By setting the name to "Vitalik" and retrieving the transaction hash, you've completed a full interaction with your Solidity contract on the Open Campus Codex network. Here's a breakdown of what occurred:

- **Transaction Creation:** When you called the `setName` function and entered "Vitalik", a transaction was created to update the `name` state variable in your contract.
- **MetaMask Confirmation:** MetaMask prompted you to confirm the transaction, ensuring you agreed to the gas fees and changes being made.
- **Transaction Execution:** Upon confirmation, the transaction was executed on the Open Campus Codex network, updating the state variable.
- **Transaction Hash:** The transaction hash was generated, serving as a unique identifier for this specific transaction. You can use this hash to track and verify the transaction on the blockchain.

### Conclusion

You've now successfully set the name to "Vitalik" in your Solidity contract and retrieved the transaction hash. This hands-on interaction helps you understand how to update state variables and track transactions on the blockchain.

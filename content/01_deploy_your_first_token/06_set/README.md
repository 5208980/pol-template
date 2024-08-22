# Interacting with Your Smart Contract

This section builds on the previous one, where we deployed a smart contract to the Open Campus Codex network. Proof of Learn (POL) provides quests that guide users through interacting with smart contracts, ensuring they gain an interactive understanding of how smart contracts work.

To start, you can find the interaction quest using the [quest.config.json template](https://github.com/5208980/pol-template/blob/master/quest.config.json).

In this guide, we'll use the `SimpleContract` you deployed in the previous section. Specifically, we'll interact with the `set` method, allowing you to change the `name` variable in the contract on the Open Campus Codex chain.

## Interacting with the Contract

Now that your contract is deployed on the Open Campus Codex network, let's interact with it by setting the `name` to `"Vitalik"` and retrieving the transaction hash. The transaction hash is a unique identifier for your transaction on the blockchain, allowing you to track and verify the transaction.

## Locate and Load the Contract

1. Use the deployed contract address to load the contract in your preferred blockchain explorer or development tool.
2. Ensure that you have the contract's ABI (Application Binary Interface) available for interacting with its functions.

## Call the `set` Method

1. Locate the `set` function in your contract interface.
2. In the input field, type `"Vitalik"` (including the quotes).
3. Click the "Transact" button to send the transaction.
4. Confirm the transaction with MetaMask or your connected wallet, then wait for the transaction confirmation.

## Check the Contract's State

1. Once the transaction is confirmed, you can check the state of the `name` variable.
2. Call the `name` function in your contract to retrieve its current value.
3. If the result is `"Vitalik"`, congratulations! You've successfully interacted with your contract.

## Submit the Transaction to POL

To validate this part of the quest, submit the transaction hash to the Proof of Learn (POL) platform. This confirms that you've successfully interacted with the smart contract.